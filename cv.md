# **Antonina Maksimova**


**Location:** Belarus, Minsk    
**tel.:** +375259240683     
**email:** tonkastar@mail.ru    
**github:** antoninamaximova    
**telegram:** amaxteam      

## SUMMARY

Web Developer with 3+ years of freelance experience in designing and developing user friendly unterfaces. 

## Tecnical Skills
* **Technologies and Frameworks:** HTML/CSS/JS, React.js, PHP.
* **Tools:** Webpack
* **CMS:** Wordpress
* **Databases:** MySQL
* **Version Control Systems:** Git
* **Integrated Development Environment:** Visual Studio code
* **Methodologies:** Scrum, Agile



## CODE REVIEW
```
let easy = document.getElementById('easy');
let medium = document.getElementById('medium');
let difficult = document.getElementById('difficult');
let button = document.getElementById ('button');
let section = document.getElementById('container');

button.addEventListener ('click', () => {
	document.querySelector('.container').classList.toggle('disable');
	let start = document.querySelector('input[type="radio"]:checked');

	section.insertAdjacentHTML('afterbegin','<div><div><div></div><div></div></div></div>');
	let cardholder = section.firstChild;
	cardholder.classList.add("cardholder");
	let playingCard = document.querySelector('.cardholder');
	let card = playingCard.firstChild;
	card.classList.add('card');
	card.firstChild.classList.add("card__font");
	card.lastChild.classList.add("card__back");
	let back = document.querySelector('.card__back');
	let clone = playingCard.cloneNode(true);
	switch(true) {
		case start == document.getElementById('medium'):
		section.classList.remove('container-easy', 'disable');
		section.classList.add('container-medium');
		for (i = 0; i < 5; i++) {
			let clone = playingCard.cloneNode(true);
			section.appendChild(clone);
		}
		break;
		case start == document.getElementById('difficult'):
		section.classList.remove('container-easy', 'disable');
		section.classList.add('container-difficult');
		for (i = 0; i < 9; i++) {
			let clone = playingCard.cloneNode(true);
			section.appendChild(clone);
		}
		break;
		default:
		section.classList.remove('disable');
		for (i = 0; i < 2; i++) {
			let clone = playingCard.cloneNode(true);
			section.appendChild(clone);
		}
	}

	let cardsMassive = Array.from(section.children);
	let randomCard = cardsMassive[Math.floor(Math.random()*cardsMassive.length)];
	randomCard.querySelector('.card__back').classList.add('card__back_win');
	randomCard.querySelector('.card__back').classList.remove('card__back');

	let cardItem = document.querySelectorAll('.card');

	cardItem.forEach(function(elem, i){
		elem.addEventListener('click', () => {
			if (elem != document.querySelector('.card__change')) {
				elem.classList.add('card__change');
			} else {
				document.querySelector('.container').classList.toggle('disable');
				section.classList.add('container-easy', 'disable');
				section.classList.remove('container-medium', 'container-difficult');
				for (i = cardsMassive.length; i > 0; i--) {
				section.removeChild(document.querySelector('.cardholder'));}
				elem.classList.remove('card__change');
			}
		});
	})
})
```

## WORK EXPERIENCE
August, 2018 untill now. Freelance practice.

### Best projects and portfolio:
[https://klubnichniyhutorok.by/]    
[https://asisukraine.org/]      
[http://nautilus-taxi.pro/] (site and calculator)   
[https://antoninamaximova.github.io/AxionShop/]     
[https://antoninamaximova.github.io/reactAppTodo/]      
[https://antoninamaximova.github.io/CardGameJS/]    
[https://antoninamaximova.github.io/turictic/]  

## EDUCATION

**Name of the Education Establishment:** BSUIR      
**Faculty/College:** Computer Systems and Networks      
**Degree (Diploma):** Uncompleted higher education      
**Specialty:** Information Technologies Software Support (Software Еngineer)    


## Trainings/Courses:
WebHeroSchool(Web Developer React)


## LANGUAGES

    English - B1(Intermediate);     
    German - A1;    
    Russian - Native.   