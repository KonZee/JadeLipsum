# Jade lipsum mixin
Lorem ipsum mixin designed for easy creatiion of random dummy-content. It can create single word with requested length or requested quantity of words, sentences and paragpraph.  
Fore beautiful result mixin create text with some visual feathures - capitalize first letter, place point or questio at the end of sentence and put some comma inside text. Number of words in sentence and sentences in paragraph are random between defined min and max value, but result is normally-distributed.

## How to use:
Add mixin in your Jade template:
```jade
include lipsum
```
Then create content what you need:
```jade
+lipsum(items, type)
```
**items** must be number.  
**type** must be on of following strings: *"characters"*, *"words"*, *"sentences"*, *"paragpraphs"*. Paragrpaphs generated inside **p** tag, all other clear from any HTML

## Usage examples
```jade
+lipsum(7, "characters") 
//- Doadipi
+lipsum(7, "characters") 
//- Mollite 
+lipsum(2, "words") 
//- Ullamco laboris
+lipsum(5, "words") 
//- Sunt dolor ipsum eu ullamco 
+lipsum(2, "sentences") 
//- Labore proident ullamco. Ex, magna in sunt deserunt fugiat, sit, deserunt commodo dolore esse dolore tempor in? 
+lipsum(2, "sentences") 
//- Anim do ut minim reprehenderit, culpa, dolore. Qui, consequat amet minim, velit occaecat, laboris nisi laborum irure. 
+lipsum(2, "paragpraphs") 
//-
	p
		Ullamco eiusmod et, occaecat aliquip tempor sunt. Ea pariatur et sed ullamco tempor tempor aliqua incididunt? 
	p
		Anim laborum, nulla aliqua culpa, deserunt, eiusmod? Labore pariatur nulla, ipsum elit reprehenderit sunt lorem minim laborum culpa, ut enim. 
```


