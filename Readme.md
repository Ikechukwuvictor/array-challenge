// solution to Array challenge

/* create a function that would be used to calculate the percentage of tip, this function takes any bill and this bill
will to  cal the percentage and  output the tips */
 function calTips(bill){
     if(bill >= 50 && bill <= 300){
         return bill * 0.15
     }
     else {
         return bill* 0.20;
     }
 }

 // we create array of the bills collected.
// we create an array tips, then use the function above to calculate the bills to get the tips
let bills  = [125, 555, 44];
 let tips = [calTips(bills[0]), calTips(bills[1]), calTips(bills[2])];
 document.write(`Bills: ${bills} and tips: ${tips}`);
//create an array Calculate to sum up bills and tips

let total = [bills[0] + tips[0], bills[1] + tips[1], bills[2] + tips[2]];
console.log(total);
