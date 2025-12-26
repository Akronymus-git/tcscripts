// ==UserScript==
// @name         New Userscript
// @namespace    http://tampermonkey.net/
// @version      2025-12-13
// @description  try to take over the world!
// @author       You
// @match        https://playtradecraft.com/app
// @icon         https://www.google.com/s2/favicons?sz=64&domain=playtradecraft.com
// @grant        none
// ==/UserScript==

(function() {
    'use strict';
    const domElement = document.createElement("button");
    domElement.classList.add("btn")
    domElement.classList.add("blue")
    domElement.id = "cancelAll"
    domElement.textContent = 'cancel all'
    const cancelAll = () => {
        let c = document.getElementsByClassName("btn xs danger cancel")
        for (let i = 0; i<c.length; i++) {
            c[i].click()}
    }
    domElement.addEventListener('click', cancelAll)
    document.querySelector("#btnTenders").parentElement.appendChild(domElement)

    let op = document.querySelector('#orderPrice')
    let ar = document.querySelector('#bandRange')
    let setmaxprice = document.createElement('button')
    setmaxprice.textContent = 'MP'
    setmaxprice.classList.add("order-btn")
    setmaxprice.addEventListener('click', () => {let op = document.querySelector('#orderPrice');let ar = document.querySelector('#bandRange');
op.value = ar.textContent.match(/- \$((?:\d|\.)*)/)[1] })
    let p = document.querySelector('#orderAmountRow')
    p.appendChild(setmaxprice)
})();
