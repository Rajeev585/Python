# `logging`

- Record `Progress` and `Problems`
- `Logs` in right place helps us to know and look at the `behaviours`, `errors` and `warnings` over time.
- Give a better overall view on order of execution and what exactly is happening inside the code step by step.


```python
import logging
```

### Standard Logging `Levels`

Each and every level is assigned with a `constant` value.

1. `DEBUG` : Detailed information, step by step processing, while diagnosing problems.
2. `INFO` : Confirmation that things are working as expected.
3. `WARNING` : Indicates that something unexpected happened, or indicate problems in near future.
4. `ERROR` : More serious problem, it may stop the process.
5. `CRITICAL` : Serious error, indicating that the program may not be able to continue running.

`Logger` will only write messages with a level `>=` set level

If we set the level to `logging.DEBUG` then we can see all log messages.

By default logging is in append mode, we can override by `filemode = 'w'`

Level | Value
:--- | :---:
NOTSET | `0`
DEBUG | `10`
INFO | `20`
`WARNING` | `30` (Default)
ERROR | `40`
CRITICAL | `50`
