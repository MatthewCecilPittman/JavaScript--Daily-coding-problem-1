# JavaScript--Daily-coding-problem-1
/* Daily coding problem #1-->
Given a list of numbers and a 
number k, return whether any 
two numbers from the list add up to k.
For example, given [10, 15, 3, 7] and
 k of 17, return true since 10 + 7 is 17.*/

function twoNumbersEqual(inList, k) {
const lookup = [];

     for (const item of inList) {
if(lookup[k - item]) {
return true;
}
lookup[item]=k - item;
}
return false;
}
console.log(twoNumbersEqual ([10,15,3,7]),17));
