# Ch9 VM as a Tool for Caching

## 9.3 Address Spaces

### 9.3.6 Locality

局部性原则保证了在任意时刻，程序将倾向于在一个较小的活动页面（active page）集合上工作，这个集合叫做工作集或者常驻集合。在初始开销，将工作集页面调度到内存中之后，接下来会对工作集的引用会命中。

抖动：工作集大小超出了物理内存大小，页面不断换入换出，导致性能变慢。