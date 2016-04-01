# hms 0.0-3 (2016-04-01)

- Implement `as.data.frame.hms()`, forwards to `as.data.frame.difftime()` (#7).
- Remove `lubridate` dependency (#8).
- Return unchanged input in `print()`.
- Inherit from `difftime` class (#6).
- Tests for arithmetic with `Date`, `POSIXt` and `hms` classes.


# hms 0.0-2 (2016-03-31)

- New `is.hms()` (#2).
- Use Travis-CI.
- Test coverage on Travis.


# hms 0.0-1 (2016-03-31)

First draft.

- Values are stored as a numeric vector that contains the number of seconds
  since midnight.
- Supports construction from time values, coercion to and from various data
  types, and formatting.
- Can be used as a regular column in a data frame.
- Full test coverage.
- Interface:
    - `hms()`
    - `as.hms()` for `character`, `numeric`, `POSIXct` and `POSIXlt`
    - `as.xxx.hms()` for `character`, `numeric` (implicitly), `POSIXct` and
      `POSIXlt`
    - `format.hms()`
    - `print.hms()`