

# Nikolai Komarov

![](https://cspromogame.ru//storage/upload_images/avatars/776.jpg)

# My contacts:
* Telegram: 87054144973
* Email: k_k_007@mail.ru
* Discord(rs-school): Nikolay (@Sancekez)

# About myself

> Hi! I am one of the most creative and sociable students at the IT University of our beautiful and sunny city of Almaty! I am studying on second year. I really like web-programming, and because of this I'd like to become a Frontend developer. I have got some experience in web-development and I have done some web-stores on vanilla js. My strong sides are knowledge Scss, Bootstrap, Figma, Photoshop, BAM methodology. My dream is working in a big IT company like PAM and I hope I will do that!

## My knowledge and skills:
1. HTML5, css3, css, js, Bootstrap, gulp, npm, GIT.
2. I'm making up the BEM methodology.
3. Block fixed / rubber layout.
4. Adaptive layout.
5. Parallax scrolling.
6. Writing simple, reliable, readable code.

## Links of my works to git:

[First project](https://sancekez.github.io/JOHN/)<br>
[Second project](https://sancekez.github.io/OXYGEN/)

## Example of my code on js:

	const todo = {
		action(e) {
			const target = e.target;

			if (target.classList.contains('todo__action')) {
				const action = target.dataset.todoAction;
				const elemItem = target.closest('.todo__item');
				if (action === 'deleted' && elemItem.dataset.todoState === 'deleted') {
					elemItem.remove();
				} else {
					elemItem.dataset.todoState = action;
				}
				this.save();
			} else if (target.classList.contains('todo__add')) {
				this.add();
				this.save();
			}
		},
		add() {
			const elemText = document.querySelector('.todo__text');

			if (elemText.disabled || !elemText.value.length) {
				return;
			}

			document.querySelector('.todo__items').insertAdjacentHTML('beforeend', this.create(elemText.value));
			elemText.value = '';
		},
		create(text) {
			return `<li class="todo__item" data-todo-state="active">
				<span class="todo__task">${text}</span>
				<span class="todo__action todo__action_restore" data-todo-action="active"></span>
				<span class="todo__action todo__action_complete" data-todo-action="completed"></span>
				<span class="todo__action todo__action_delete" data-todo-action="deleted"></span></li>`;
		},
		init() {
			const fromStorage = localStorage.getItem('todo');
			if (fromStorage) {
				document.querySelector('.todo__items').innerHTML = fromStorage;
			}
			document.querySelector('.todo__options').addEventListener('change', this.update);
			document.addEventListener('click', this.action.bind(this));
		},
		update() {
			const option = document.querySelector('.todo__options').value;
			document.querySelector('.todo__items').dataset.todoOption = option;
			document.querySelector('.todo__text').disabled = option !== 'active';
		},
		save() {
			localStorage.setItem('todo', document.querySelector('.todo__items').innerHTML);
		}
	 };

	 todo.init();
 

## My level of English is pre-intermediate. At the university we study in Russian and English!
