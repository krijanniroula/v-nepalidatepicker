# nepali-datepicker-vuejs

> An easy-to-use and customizable nepali date picker component powered by Vue js

# Demo: 

![Demo1](https://github.com/krijanniroula/v-nepalidatepicker/blob/master/assets/demo1.PNG)    ![Demo2](https://github.com/krijanniroula/v-nepalidatepicker/blob/master/assets/demo2.PNG)


## Install
```shell
npm install v-nepalidatepicker
```

## Quick Start
``` javascript
import VNepaliDatePicker from 'v-nepalidatepicker';

export default {
  components: {
    VNepaliDatePicker,
  },
  // rest of the component
}

Or even used via <script> tag in the browser directly:

<script src="https://unpkg.com/vue"></script>
<script src="https://unpkg.com/v-nepalidatepicker"></script>
...
<v-nepalidatepicker />
...

```

## Customizable Properties

The following customizable properties can be added to the component

1. classValue 
2. calenderType
3. placeholder
4. format
5. value
6. yearSelect
7. monthSelect

## Examples - classValue

This works exactly as class properties. Eg: classValue="form-control"

```vue
<template>
  <v-nepalidatepicker classValue="datepicker" />
</template>
<style>
.datepicker{
  width: 50px;
  height: 20px;
}
</style>
```


## Examples - calenderType

Date picker is present in nepali language and English nepali language. 
Default type will be English nepali.

For nepali language : 

```vue
<template>
  <v-nepalidatepicker calenderType="Nepali" />
</template>

```

## Examples - placeholder

```vue
<template>
  <v-nepalidatepicker placeholder="YYYY-MM-DD" />
</template>

```

## Examples - format

Format the date to provide various output based on format string

```vue

'yyyy-mm-dd' => २०७५-०२-०१
'YYY-MM-DD' => 075-02-01
'mmmm d, yyyy ddd' => जेष्ठ १, २०७५ मंगल
'MMM D, YYYY DDD' => Jes 1, 2075 Tue

```

```vue

YYYY - 4 digit of year (2075)
yyyy - 4 digit of year in nepali unicode (२०७५)
YYY  - 3 digit of year (075)
yyy  - 3 digit of year (०७५)
YY   - 2 digit of year
yy   - 2 digit of year in nepali unicode (७५)
M    - month number (1 - 12)
m    - month number (१ - १२) in nepali unicode
MM   - month number with 0 padding (01 - 12)
mm   - month number in nepali unicode with 0 padding - (०१-१२)
MMM  - short month name (Bai, Jes, Asa, Shr, etc.)
mmm  - short month name in nepali unicde (ब‍ै, जे, अ, श्रा, etc)
MMMM - full month name (Baisakh, Jestha, Asar, ...)
mmmm - full month name nepali (बैसाख, जेष्ठ, ...)
D    - Day of Month (1, 2, ... 31, 32)
d    - Day of Month in Nepali unicode (१, २, ३ ... ३१, ३२)
DD   - Day of Month with zero padding (01, 02, ...)
dd   - Day of Month with zero padding in Nepali unicode (०१, ०२, ...)
DDD  - Day of Week short form (Sun, Mon, Tue, ...)
ddd  - Day of week in short form nepali (आइत, सोम, ...)
DDDD - Day of week full form (Sunday, Monday, Tuesday, ...)
dddd - Day of week full form nepali (आइतबार, सोमबार, ...)

```

```vue
<template>
  <v-nepalidatepicker format="YYYY-MM-DD" />
</template>

```

## Examples - value

Initial value for the datepicker.

```vue
<template>
  <v-nepalidatepicker value="2053-09-19" />
</template>

```

## Examples - yearSelect

The dropdown year select can be turned off using boolean type to yearSelect

```vue
<template>
  <v-nepalidatepicker :yearSelect="false" />
</template>

```

## Examples - monthSelect

The dropdown month select can be turned off using boolean type to monthSelect

```vue
<template>
  <v-nepalidatepicker :monthSelect="false" />
</template>

```

## Examples - All in one

```vue
<template>
  <v-nepalidatepicker calenderType="Nepali" placeholder="YYYY-MM-DD" format="YYYY-MM-DD" value="2053-09-19" :yearSelect="false" :monthSelect="false" />
</template>

```
