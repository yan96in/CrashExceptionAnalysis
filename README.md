# CrashExceptionAnalysis
对于一款App而言，最重要的莫过于稳定性，没有之一。<br/>
Android之所以存在千奇百怪的Crash，主要归结于以下几种情况：<br/>
1）Android系统的碎片化。各种硬件厂商都定制自己的ROM，改写了Android系统的很多方法。对于App而言，在大多数手机<br/>
上没问题，但是到了该厂商的手机系统里，使用到这些方法就会崩溃。当然，也不排除ROM上的方法被改写后存在bug的情况。<br/>
2）MobileAPI返回了脏数据。比如说当MobileAPI返回空值或空数组时，App收到数据后就会发生空指针或数组越界的Crash。有时
则是某个字段返回0，而这个字段作为除数时，也会发生不能为0的Crash。

