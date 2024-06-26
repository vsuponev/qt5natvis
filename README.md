# qt5natvis
All .natvis files for Qt5 that I have ever found didn't represent certain types properly in CLion (and probably in other IDEs too).

Fixes:
* The `AlternativeType` tag doesn't seem to work well. All entries that had aliases declared this way were extracted into standalone entries. This affects type like `QStringList`.
* Convenient fast lookup added to smart pointers as `Value`. It won't be shown for null pointers.
