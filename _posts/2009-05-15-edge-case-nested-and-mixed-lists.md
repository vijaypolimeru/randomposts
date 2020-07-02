---
title: "Edge Case: Nested and Mixed Lists"
categories:
  - Edge Case
tags:
  - content
  - css
  - edge case
  - lists
  - markup
last_modified_at: 2017-03-09T14:25:52-05:00
---



<div class="card mb-3" style="max-width: 100%;">
  <div class="row no-gutters">
    <div class="col-md-4">
      <img src="https://vijaypolimeru.github.io/images/vijay-polimeru.jpg" class="card-img" alt="my_photo">
    </div>
    <div class="col-md-8">
      <div class="card-body">
        
		<h1 id="page-title" class="card-title page-title" style="font-size: 2.5em;">Vijay Kumar Polimeru</h1>
        <p class="card-text" style="font-size: 1.2em;">Research Scholar (Ph. D) <br>Department of Civil Enigneering <br>
		IIT Bombay <br> 
		Powai, Mumbai, Maharashtra, India, 400076<br>
		Email : <span style="font-size: 0.9em;"><em>vijaykumarpolimeru@iitb.ac.in </em> </span>  <br> 
			<span style="text-indent: -20em;padding-left: 2.7em;">: <em><span style="font-size: 0.9em;">polimeru.vijaykumar@gmail.com</span></em> </span> <br> 

		</p>	
			
        </div>
    </div>
  </div>
</div>



Nested and mixed lists are an interesting beast. It's a corner case to make sure that lists within lists do not break the ordered list numbering order and list styles go deep enough.

## Ordered -- Unordered -- Ordered

1. ordered item
2. ordered item 
  * **unordered**
  * **unordered** 
    1. ordered item
    2. ordered item
3. ordered item
4. ordered item

## Ordered -- Unordered -- Unordered

1. ordered item
2. ordered item 
  * **unordered**
  * **unordered** 
    * unordered item
    * unordered item
3. ordered item
4. ordered item

## Unordered -- Ordered -- Unordered

* unordered item
* unordered item 
  1. ordered
  2. ordered 
    * unordered item
    * unordered item
* unordered item
* unordered item

## Unordered -- Unordered -- Ordered

* unordered item
* unordered item 
  * unordered
  * unordered 
    1. **ordered item**
    2. **ordered item**
* unordered item
* unordered item
