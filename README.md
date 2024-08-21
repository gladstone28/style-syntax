[Link to lesson](https://www.codecademy.com/courses/react-101/lessons/react-style/exercises/style-name-syntax)

### React Styles

**Style Syntax**

There are a few things to keep in mind when styling components with JSX.

Just like how we reference CSS properties in the style object of the DOM in JavaScript, we write CSS property names using camelCase in React:
```
const styles = {
  marginTop: '20px',
  backgroundColor: 'green'
};
```

This syntax comes from a small rule. A hyphen is a reserved operator in JavaScript. If we use background-color, the hyphen is then interpreted as a minus sign. Thus, we want to be consistent with the property names in the DOM style JavaScript object and use camel case.

In regular JavaScript, style values are almost always strings. Even if a style value is numeric, you usually have to write it as a string so that you can specify a unit. For example, you’d write '450px' or '20%'.

If you write a style value as a number, then the unit 'px' is assumed. For example, if you want a font size of 30px, you can write:
```
{ fontSize: 30 }
```
If you want to use units other than 'px', you can use a string:
```
{ fontSize: "2em" }
```
Specifying the 'px' unit in a string will still work, although it’s redundant.

A few specific styles will not automatically fill in the px for you. These are styles where you aren’t likely to use 'px' anyway, so you don’t really have to worry about them.

