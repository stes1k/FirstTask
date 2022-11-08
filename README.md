let Armstrong = (arr) => {
    let OldArr = arr.join().split('')
    let NewArr = OldArr.map((el) => Math.pow(Number(el), OldArr.length))
    let SumNewArr = NewArr.reduce((sum, current) => sum + current, 0)
    arr.map((el) => Number(el))
    return arr == SumNewArr
}
console.log(Armstrong([371]))
console.log(Armstrong([7]))
console.log(Armstrong([1938]))
