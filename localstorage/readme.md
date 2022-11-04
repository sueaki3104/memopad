- 課題提出用は　localstorage　→　memo課題ver1　です


// ユーザーデータ
localStorage.setItem("user.name", "panda");
localStorage.setItem("user.age",  "15");

// 履歴
localStorage.setItem("history.page", "/home/page");
localStorage.setItem("history.date", "2020-08-13");


// JSON.stringify()でJSON文字列化
localStorage.setItem("test1", JSON.stringify(123));
localStorage.setItem("test2", JSON.stringify(true));
localStorage.setItem("test3", JSON.stringify([1,2,3]));
localStorage.setItem("test4", JSON.stringify({"a":"foo", "b":"bar"}));

// JSON.parse()で元に戻す
console.log(
  JSON.parse(localStorage.getItem("test1")),  // 123
  JSON.parse(localStorage.getItem("test2")),  // true
  JSON.parse(localStorage.getItem("test3")),  // [1,2,3]
  JSON.parse(localStorage.getItem("test4"))   // {"a":"foo", "b":"bar"}
);