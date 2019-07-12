function anagrams(word, words) {
  function isAnagram(str){
    return str.split("").sort().join("") === word.split("").sort().join("");
  }
  return words.filter(a => isAnagram(a));
}