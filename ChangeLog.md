  * row\_cache\_for\_mysql.5.1.48\_2012\_03\_22.diff
    * 避免truncate只改变tablei\_id不改变index\_id导致row cache不失效的bug
  * row\_cache\_for\_mysql.5.1.48\_2012\_03\_01.diff
    * fix bug 回滚需在btr\_pcur\_restore\_position确认pcur之后 再remove row cache 否则可能会因为pcur错位而导致crash
  * row\_cache\_for\_mysql.5.1.48\_2012\_01\_11.diff
    * 修复一个幻读的bug
  * row\_cache\_for\_mysql.5.1.48\_2011\_09\_27.diff
    * 修复了一个由于错误缓存了被逻辑删除的记录导致的crash bug
  * row\_cache\_for\_mysql.5.1.48\_2011\_06\_16.diff
    * 提供innodb\_row\_cache\_additional\_mem\_pool\_size 优化小内存分配
    * 提供innodb\_row\_cache\_index 可针对具体索引进行缓存
    * 提供innodb\_row\_cache\_clean\_cache 可清缓存
    * 提供innodb\_row\_cache\_use\_sys\_malloc 可利用系统malloc进行内存分配
  * row\_cache\_for\_mysql.5.1.48\_2011\_05\_11.diff
    * 初始版本