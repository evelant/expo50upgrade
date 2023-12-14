`pnpm install`

`pnpm expo start`

`eas build -p ios --profile development --local`

fails to compile due to header paths issue

```
[RUN_FASTLANE] › Compiling .pnpm Pods/Yoga » PixelGrid.cpp
[RUN_FASTLANE]
❌  (node_modules/.pnpm/react-native@0.73.0_@babel+core@7.23.6_@babel+preset-env@7.23.6_react@18.2.0/node_modules/react-native/ReactCommon/yoga/yoga/algorithm/PixelGrid.cpp:10:10)

   8 | #include <yoga/Yoga.h>
   9 |
> 10 | #include <yoga/algorithm/PixelGrid.h>
     |          ^ 'yoga/algorithm/PixelGrid.h' file not found
  11 | #include <yoga/numeric/Comparison.h>
  12 |
  13 | namespace facebook::yoga {
```
