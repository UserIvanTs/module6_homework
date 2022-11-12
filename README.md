Задание 1

let arr = [13, 22, 37, 46, 0.4, 1.7, null, 66, undefined, 55, 44, 0];
function getOddandEvenCountArray(arr) {
    let zerocount = 0;
    let numbercount = 0;
    let evencount = 0;
    let oddcount = 0;
   for (let i = 0; i < arr.length; i++) {
        if (typeof arr[i] === "number" ||!isNaN(arr[i])) {
            numbercount += 1;
            if (arr[i] === 0) {
                zerocount += 1;
            } else if (arr[i] % 2 === 0) {
                evencount += 1;
            } else {
                oddcount += 1;
            }
        }
    }
    
    console.log(`В массиве ${zerocount} нулей, ${evencount} чётных, ${oddcount} нечётных!`);
}
   getOddandEvenCountArray(arr);

Задание 2


