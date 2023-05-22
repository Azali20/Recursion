function isPalindrome(arra) {
  // Initialize counters and indices
  const left = 0;
  const right = word.length - 1;

  // Iterate until the indices meet or cross each other
  
  while (left < right) {
    // Compare characters at the ends
    
    if (word[left] !== word[right]) {
      return false; // Characters are different, not a palindrome
    }

    // Move the counters inward
    left++;
    right--;
  }

  // All characters matched, it's a palindrome
  return true;
}

// Example usage
const word = prompt("Enter a word: ");
if (isPalindrome(word)) {
  console.log("The word is a palindrome.");
} else {
  console.log("The word is not a palindrome.");
}


In this updated code, the isPalindrome function uses two counters (left and right) to iterate over the word. It starts with left at the beginning of the word and right at the end of the word. The function enters a while loop that continues until the left and right indices meet or cross each other.

Inside the loop, it compares the characters at the ends of the word using the inequality (!==) operator. If the characters are different, it returns false indicating that the word is not a palindrome. Otherwise, it moves the counters inward by incrementing left and decrementing right.

Once the loop finishes, if all characters have been matched (i.e., left and right have crossed each other), it returns true, indicating that the word is a palindrome.

You can run this code in a JavaScript environment or a browser, and it will prompt you to enter a word. Then it will output whether the word is a palindrome or not based on the implemented counters and loops logic.
