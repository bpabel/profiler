Tools to easily profile python code and view results.

Basic usage

```python
import profiler
profiler.profiler().start(True)
```

Profiling will automatically end when python exits and open the results with the default text editor.

Alternatively, you can perform profiling manually.

```python
import profiler
p = profiler.profiler()
p.start()
print("All code called after start will be profiled")
p.end()
```

The Profiler can also be used as a context manager.

```python
import profiler
with profiler.profiler():
    print("Code in here will be profiled")
```

In each example, profile results will automatically be opened in the default text editor when profiling completes.
