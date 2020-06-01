# Playground-
function checkPalindrome(str){
  let le = str.length;
  if (le === 0 || le === 1) {
    return true;
  }
  if (str[0] === str[le - 1]) {
    return checkPalindrome(str.slice(1, le - 1) );
  }  
  return false;
};
//0.30 ms
function checkPalindrome(str){
  let reversed = str.split("").reverse().join("")
  return str === reversed
}
let str1 = "anna"
let str2 = "banana"
let str3 = "kayak"
checkPalindrome(str1)
// -> true
checkPalindrome(str2)
// -> false
checkPalindrome(str3)
// -> true
//0.52 ms
function checkPalindrome(str) {
 let l = str.length;
 for (let i = 0; i < l/2; i++) {
  if (str[i] !== str[l - 1 - i]) {
   return false;
  }
 }
 return true;
}
//0.20 ms
