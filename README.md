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

It uses format type as per following documentation:

<p align="center">
  <a href="https://github.com/sharingapples/nepali-date#readme">
  <h2>View Docs</h2>
  </a>
</p>

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
