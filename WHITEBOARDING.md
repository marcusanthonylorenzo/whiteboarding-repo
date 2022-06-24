//deleted previous content to do whiteboarding without resources


Question #4: Checking for Uniqueness
Write an algorithm that determines whether all the elements in a string are unique.
You may not convert the string into an array or use array methods to solve this problem.

The algorithm should return a boolean.

/***
input: string


output: boolean
  return true
  return false

***/


const checkString = (string) => {
  for (let i = 0; i < string.length; i++) {
    for (let j = 1; j < string.length; j++) {
      if (str[i] === str[j]){
        return false
      }
    }
   return true
  }
}
checkString();

