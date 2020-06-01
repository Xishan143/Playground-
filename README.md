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
