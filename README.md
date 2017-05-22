# PhpStorm Live Templates
## Installation

First, find your PhpStorm templates folder. It contains XML files with Live Templates. It will be something like this:
```
Windows: <your home directory>/.PhpStorm<version>/config/templates
Linux: ~/.PhpStorm<version>/config/templates/
```
Create a git repository in it and pull the templates.
```
$ cd ~/.PhpStorm2017.1/config/templates/
$ git init
$ git remote add origin git@github.com:jiriferkl/phpstorm-livetemplates.git
$ git pull origin master
```
## Manual
### Doctrine
Comments in annnotations are just for better imagination when programming. You can delete them.
#### mto
```php
class Ingredient
{

	/**
	 * @var Recipe
	 * Many Ingredients have One Recipe.
	 * @ORM\ManyToOne(targetEntity="Recipe", inversedBy="ingredients")
	 */
	private $recipe;
}

```
#### otm
```php
class Recipe
{

	/**
	 * @var Ingredients[]|Collection
	 * One Recipe has Many Ingredients.
	 * @ORM\OneToMany(targetEntity="Ingredients", mappedBy="recipe")
	 */
	private $ingredients;

}

```


There is many more but doc is missing! Sorry I will do it later.
