//async await
async function async1() {
    setTimeout(() => {
        console.log("async1执行完毕");
    }, 1000);
}
async1(); //async1执行完毕
console.log(async1()); //Promise{}
//await //捕获异常
async function async2() {
    let result3 = await async3();
    try {
        let result4 = await async4();
    } catch (e) {
        console.log(e); //执行错误
    }

    console.log(result3); //10
    //console.log(result4);//8
}
async function async3() {
    return new Promise((resolve) => {
        resolve(10);
    });
}
async function async4() {
    return new Promise((resolve, rejecte) => {
        // resolve(8);
        rejecte("执行错误");
    });
}
async2(); //10 8
