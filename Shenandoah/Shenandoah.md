# Shenandoah GC Settings

## Shenandoah GC Visualizer

* Clone the repo from https://github.com/openjdk/shenandoah-visualizer
* cd into it
* `mvn clean verify`
* Go to `target` and start the jar

```
java -jar .\visualizer.jar local://13228
```

## Shenandoah in JMeter

* Add the below arguments in `GC_ALGO` var in `jmeter.bat`:

```
-XX:+UseShenandoahGC -XX:+UsePerfData -XX:+UnlockExperimentalVMOptions -XX:+ShenandoahRegionSampling
```