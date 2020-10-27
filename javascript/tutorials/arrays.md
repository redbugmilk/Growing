# Arrays

## How to remove null entries in an array

```javascript
const arrayOfNumbers = [1, { a: "RedBug", b: "Milk" }, 4, '', null, 2, 0, null, "Milk"];
const arrayClean = arrayOfNumbers.filter(Boolean);
```

## How to remove duplicates in array

### Remove unique values

```javascript
const arrayOfNumbers = [1, 2, 3, 4, 5, 1, 2, 3, 4];
const setWithRemovedEntries = new Set(arrayOfNumbers);
const arrayOfNumbersWithRemovedEntries = [...setWithRemovedEntries];
```

### Remove inside objects with equal parameters

```javascript
const arrayOfNumbers = [
  { a: "RedBug", b: "Milk" },
  { a: "WhiteBug", b: "Milk" },
  { a: "Donald", b: "Duck" },
];
const removeDuplicated = arrayOfNumbers.filter(
  (entries, index, self) =>
    index === self.findIndex((item) => item.b === entries.b)
);
```
