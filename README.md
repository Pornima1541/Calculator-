<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
  </head>
  <body class="flex justify-center items-center h-[100vh] bg-gray-100">
    <div class="border p-5 text-center w-[50%] rounded-lg shadow-sm bg-blue-100">
        <p class="text-5xl mb-5">
            Calculator
        </p>
        <input type="text" class="rounded-t-lg w-full border h-14 text-2xl p-3 bg-gray-50" disabled id="res" >

        <div class="border border-t-0 rounded-b-lg text-2xl grid grid-cols-4 gap-2 font-bold  p-1 bg-blue-50">
            <button onclick="f1('1')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">1</button>


            <button onclick="f1('2')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">2</button>
            <button onclick="f1('3')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">3</button>
            <button onclick="f1('+')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">+</button>
            <button onclick="f1('4')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">4</button>
            <button onclick="f1('5')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">5</button>
            <button onclick="f1('6')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">6</button>
            <button onclick="f1('-')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">-</button>
            <button onclick="f1('7')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">7</button>
            <button onclick="f1('8')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">8</button>
            <button onclick="f1('9')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">9</button>
            <button onclick="f1('*')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">x</button>
            <button onclick="allClear()" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">AC</button>
            <button onclick="f1('0')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">0</button>
            <button onclick="f1('.')" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">.</button>
            <button onclick="showResult()" class="bg-blue-500 p-2 rounded-lg cursor-pointer text-white">=</button>
        </div>
    </div>


    <script>
        let res=document.getElementById("res")
        function f1(text){
            res.value+=text
        }
        function allClear(){
            res.value=""
        }
        function showResult(){
            res.value=eval(res.value)
        }

    </script>
</body>
</html>
