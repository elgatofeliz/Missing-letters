# Missing-letters

FreeCodeCamp
    JavaScript Algorithms and Data Structures
    Intermediate Algorithm Scripting

Missing letters

Find the missing letter in the passed letter range and return it.

If all letters are present in the range, return undefined.

--- Here's the Code ---

function fearNotLetter(str) {

  for(let i = 0; i < str.length; i++){
    if(str.charCodeAt(i) + 1 !== str.charCodeAt(i+1)){
      return str.length >= 26 ? undefined :  String.fromCharCode(str.charCodeAt(i)+1)
    }
  }
  return undefined
}

fearNotLetter("abcdefghijklmnopqrstuvwxyz");
