"use strict";

{
  // 信号機
  const blue = document.querySelector("#blue");
  const yellow = document.querySelector("#yellow");
  const red = document.querySelector("#red");
  const btn = document.querySelector("#btn");

  btn.addEventListener("click", () => {
    btn.disabled = true;
    btn.textContent = 'お待ち下さい';
    setTimeout(() => {
      red.classList.add("gray-color");
      blue.classList.remove("gray-color");
      blue.classList.add("blue-color");
      btn.textContent = '横断中';
    }, 2000);
    setTimeout(() => {
      blue.classList.add("blue-blink");
      btn.textContent = '信号が変わります';
    }, 5500);
    setTimeout(() => {
      blue.classList.remove("blue-blink");
      blue.classList.add("gray-color");
      yellow.classList.remove("gray-color");
      yellow.classList.add("yellow-color");
    }, 8500);
    setTimeout(() => {
      yellow.classList.remove("yellow-color");
      yellow.classList.add("gray-color");
      red.classList.remove("gray-color");
      red.classList.add("red-color");
      btn.disabled = false;
      btn.textContent = '押してください';
    }, 11000);
  });

  // カレンダー
  function setDay() {
    let d = new Date();
    let year = d.getFullYear();
    let month = String(d.getMonth() + 1).padStart(2, 0);
    let day = String(d.getDate()).padStart(2, 0);
    let date = `${year}年${month}月${day}日`;
    document.querySelector("#day").textContent = date;
  }

  setDay();

  // 曜日
  function setWeek() {
    let d = new Date();
    let week = d.getDay();
    let weekArray = ["(日)", "(月)", "(火)", "(水)", "(木)", "(金)", "(土)"];
    document.querySelector("#week").textContent = weekArray[week];
  }

  setWeek();

  // 時計
  function setTime() {
    let d = new Date();
    let h = String(d.getHours()).padStart(2, 0);
    let m = String(d.getMinutes()).padStart(2, 0);
    let s = String(d.getSeconds()).padStart(2, 0);
    let time = `${h}:${m}:${s}`;
    document.querySelector("#clock").textContent = time;
  }

  setTime();
  setInterval(() => {
    setTime();
  }, 100);
}
