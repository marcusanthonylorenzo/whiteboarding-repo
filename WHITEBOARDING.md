## This is where I will do the majority of my whiteboarding, hopefully it is clean and accessible this way.

Question 1: Turning Strings to URLs

const stringToURL = (string) => {

  //split this guy
  const stringToArray = string.split("");
  
  //I believe .map takes 3 arguements (element in array, index, original array to be used later)
  const newArray = stringToArray.map( (char, i) => {
  
  //shallow copy? return spliced into shallow copy then return shallow copy?
    const arrayToReturn = stringToArray;
    if (char === " "){
      arrayToReturn.splice(i, 1, "%20");
    }
    return arrayToReturn;
  })
  
  //unsplit with no spaces aka .join
  
  return newArray.join("");
}
stringToURL();
