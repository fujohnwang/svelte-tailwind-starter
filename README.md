# Intro

a scaffolding project for svelte and tailwindcss + daisyui

# to add theme change 

默认使用daisyui的luxury主题：


```html
<html lang="en" data-theme="luxury">
...
```


如果想允许用户可以切换不同的theme， 可以考虑使用[theme-change](https://github.com/saadeghi/theme-change)

```html
<script>
	import { themeChange } from 'theme-change'
	...
    onMount(async () => {
        themeChange(false)
		...
    })
</script>

<select id="theme-select" data-choose-theme class="select">
	<option value="Business">Default</option>
	<option value="dark">Dark</option>
	<option value="dracula">Dracula</option>
	<option value="luxury">luxury</option>
	<option value="Coffee">Coffee</option>
</select>
```

`data-choose-theme` is the key!


# DaisyUI 

https://daisyui.com/components/





