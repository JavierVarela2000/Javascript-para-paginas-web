const btnMenu = document.querySelector(".btnMenu");
const menu = document.querySelector(".menuContainer");

let clickMenu = true;


//Scroll menu


let prevScrollPos = window.pageYOffset;
let nav = document.querySelector("nav")
window.onscroll = enableScroll();
enableScroll();

btnMenu.addEventListener("click", function () {
  console.log(clickMenu);

  menu.classList.toggle("mostrar");
  if (clickMenu) {
    disableScroll();
    clickMenu = false;
  }
  else {
    enableScroll();
    clickMenu = true;

  }

});







function disableScroll() {
  var x = window.scrollX;
  var y = window.scrollY;
  window.onscroll = function () { window.scrollTo(x, y) };
}

function enableScroll() {
  window.onscroll = () => {

    //Hide & Show - Scroll Menu (Function)
    let currentScrollPos = window.pageYOffset;

    if (prevScrollPos > currentScrollPos) {
      nav.style.top = '0px';
      nav.style.transition = '0.5s';
    } else {
      if (clickMenu) {
        nav.style.top = '-60px';
        nav.style.transition = '0.5s';
      }
    }
    prevScrollPos = currentScrollPos;
  }
}
