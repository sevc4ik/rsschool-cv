# Savely Stefanovich

## Contatcs:

* **Location:** Hrodna, Belarus
* **E-mail:** sevka.st@gmail.com
* **Telegram:** @sevc4ik
* **Phone:** +375 29 888 78 89

## About Me:

Hello, my name is Savely. Now I work as a UX designer, but I am also interested in Front End development. Therefore, my goal is to improve my technical skills and get new skills.

## Skills:

* HTML
* CSS
* JS
* knockout.js
* UX & UI design
* GIT

## Code Example:

```
self.createAvatar = function (e) {
    let avatar = self.dragObject.elem;
    let old = {
        parent: avatar.parentNode,
        nextSibling: avatar.nextSibling,
        position: avatar.position || '',
        left: avatar.left || '',
        top: avatar.top || '',
        width: avatar.width|| '',
        zIndex: avatar.zIndex || ''
    };

    avatar.rollback = function () {
        old.parent.insertBefore(avatar, old.nextSibling);
        avatar.style.position = old.position;
        avatar.style.left = old.left;
        avatar.style.top = old.top;
        avatar.style.width = old.width;
        avatar.style.zIndex = old.zIndex;
        avatar.style.transform = '';
    };

    return avatar;
}

self.startDrag = function (e) {
    let avatar = self.dragObject.avatar;
    
    avatar.style.width = self.dragObject.avatar.offsetWidth - 22 + 'px'; 
    document.body.appendChild(avatar);
    avatar.style.zIndex = 9999;
    avatar.style.position = 'absolute';
    avatar.style.transform = 'rotate(5deg)';
}

self.findDroppable = function (event) {
    self.dragObject.avatar.hidden = true;

    let elem = document.elementFromPoint(event.clientX, event.clientY);

    self.dragObject.avatar.hidden = false;

    if (elem == null) {

        return null;
    }

    return elem.closest('.droppable');
}

self.getCoords = function (elem) {
    let box = elem.getBoundingClientRect();

    return {
        top: box.top + pageYOffset,
        left: box.left + pageXOffset
    };
};
```

## Experience:

2018 - April 2021
**Velox Imaging** HTML-coder

May 2021 - present
**Velox Imaging** UX designer

## Education:

2015-2019
**YANKA KUPALA STATE UNIVERSITY OF GRODNO,**
Bachelor, Mathematics and Computer Science

## Languages:

* Russian _native_
* English _B2_

## Hobbies:

* Music
* Cybersport
* Photography