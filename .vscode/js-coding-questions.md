1. Find duplicate element in an Array
2. Remoe duplicate element from Array
3. Find max and second max
4. str Anagram
5. str palindrome
6. reverse str
7. a = 123; sum of all ?
8. flat array
9. shifting array element with given position

10. Clone an object (shallow and deep)

// Shallow clone
const clone = { ...original };

// Deep clone
const deepClone = JSON.parse(JSON.stringify(original));

2. Check if an object is empty

function isEmpty(obj) {
return Object.keys(obj).length === 0;
}

3. Convert an object to an array of key-value pairs

Object.entries({ a: 1, b: 2 }); // [["a", 1], ["b", 2]]

4. Convert key-value pairs back to an object

Object.fromEntries([["a", 1], ["b", 2]]); // { a: 1, b: 2 }

5. Merge two objects

const merged = { ...obj1, ...obj2 };

6. Access nested object properties safely

const value = obj?.a?.b?.c;

📚 Array Manipulation Questions

7. Flatten a nested array

const flat = arr.flat(Infinity);

8. Group array items by property

function groupBy(arr, key) {
return arr.reduce((acc, obj) => {
const val = obj[key];
acc[val] = acc[val] || [];
acc[val].push(obj);
return acc;
}, {});
}

9. Find unique values

[...new Set([1, 2, 2, 3])]; // [1, 2, 3]

10. Remove falsy values from an array

[0, "", null, undefined, false, 5].filter(Boolean); // [5]

11. Sort an array of objects

arr.sort((a, b) => a.age - b.age);

12. Chunk an array into smaller arrays

function chunk(arr, size) {
let result = [];
for (let i = 0; i < arr.length; i += size) {
result.push(arr.slice(i, i + size));
}
return result;
}

🧵 String Manipulation Questions 13. Reverse a string

str.split('').reverse().join('');

14. Capitalize the first letter of each word

str.replace(/\b\w/g, char => char.toUpperCase());

15. Check if a string is a palindrome

function isPalindrome(str) {
return str === str.split('').reverse().join('');
}

16. Count character frequency in a string

function charCount(str) {
return [...str].reduce((acc, char) => {
acc[char] = (acc[char] || 0) + 1;
return acc;
}, {});
}

17. Find the longest word in a string

function longestWord(str) {
return str.split(' ').reduce((a, b) => (a.length > b.length ? a : b));
}

18. Remove duplicate characters from a string

[...new Set(str)].join('');
