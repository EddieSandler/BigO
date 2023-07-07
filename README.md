# BigO

1) O(n)
2) O(n)
3) O(1)
4) O(n^3)
5) O (n)
6) O(n)
7)O (nlogN)
8)O(2^n2)
9)O(1)



part 2

function logUpTo(n) {
  for (let i = 1; i <= n; i++) {
    console.log(i);
  }
}

Answer:
1) O (n)


function logAtLeast10(n) {
  for (let i = 1; i <= Math.max(n, 10); i++) {
    console.log(i);
  }
}

Answer: O(n)


function logAtMost10(n) {
  for (let i = 1; i <= Math.min(n, 10); i++) {
    console.log(i);
  }
}

Answer: 0(n)

function onlyNumsAtEvenIndexes(nums) {
  let numsAtEvens = [];

  for (let i = 0; i < nums.length; i++) {
    if (i % 2 === 0) {
      numsAtEvens.push(nums[i]);
    }
  }

  return numsAtEvens;
}

answer: 0(n)

function runningSubtotals(nums) {
  let subtotals = []; //1

  for (let i = 0; i < nums.length; i++) { // nums.length times
    let subtotal = 0;
    for (let j = 0; j <= i; j++) {
      subtotal += nums[j];
    }
    subtotals.push(subtotal);
  }
  return subtotals;
}

Answer: 0(n^2)

const VOWELS = "aeiouAEIOU";

function vowelsCounts(word) {
  let vowelsToCounts = {};

  for (let char of word) {
    if (VOWELS.includes(char)) { //O(n)
      if (char in vowelsToCounts) {
        vowelsToCounts[char] += 1;
      } else {
        vowelsToCounts[char] = 1;
      }
    }
  }

  return vowelsToCounts;
}

Answer: 0(n)



part 3
1)true
2)false
3)false
4)O(n)
5) O(n)
6)O(n)
7)O(nLogn)
8)O(n)
9)O(n)
10)O(n)
11) O(n)
