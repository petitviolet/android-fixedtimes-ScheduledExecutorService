# FixedTimesScheduledExecutorService

You can run task (Runnable or Callable) on worker thread specifying execution schedule like ScheduledExecutorService, and also specifying execution times.

# Interfaces

```java
ScheduledFuture<?> schedule(Runnable command, int executeTime, long delay, TimeUnit unit) {}

ScheduledFuture<?> schedule(Runnable command, int executeTime, long delay, TimeUnit unit, FixedTimesTaskListener listener) {}

<V> ScheduledFuture<V> schedule(Callable<V> callable, int executeTime, long delay, TimeUnit unit) {}

<V> ScheduledFuture<V> schedule(Callable<V> callable, int executeTime, long delay, TimeUnit unit, FixedTimesTaskListener listener) {}

ScheduledFuture<?> scheduleAtFixedRate(Runnable command, int executeTime, long initialDelay, long period, TimeUnit unit) {}

ScheduledFuture<?> scheduleAtFixedRate(Runnable command, int executeTime, long initialDelay, long period, TimeUnit unit, FixedTimesTaskListener listener) {}

ScheduledFuture<?> scheduleWithFixedDelay(Runnable command, int executeTime, long initialDelay, long delay, TimeUnit unit) {}

ScheduledFuture<?> scheduleWithFixedDelay(Runnable command, int executeTime, long initialDelay, long delay, TimeUnit unit, FixedTimesTaskListener listener) {}
```

# How to Use

```groovy
repositories {
        maven { url "https://jitpack.io" }
}
compile 'com.github.petitviolet:android-fixedtimes-ScheduledExecutorService:0.0.1'
```

# Lisence

```
Copyright 2015 @petitviolet

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```
