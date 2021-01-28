# PCXML_Documentation

PCXML is a proprietary file type, which is used in Alteryx Designer and has some similarities to HTML<br>
This document tries to get a quick, but not complete overview over pcxml.<br>
No warranties. All data are reverse engineered.
<br><br>
Version of Alteryx Designer used: 2020.2.3

# Root elements
Following elements can be used as root elements
+ [\<div>](#div)
+ [\<hX>](#hX)
+ [\<span>](#span)
+ [\<table>](#table)
+ String literal

***

## \<table>

HTML element

**Attributes:**
+ cellpadding
+ cellspacing
+ rowsContained
+ [style](#style-attribute)
+ width

**Childs:**
+ [\<thead>](#thead) (First child only)
+ [\<tbody>](#tbody)
+ [\<tr>](#tr)

***

## \<tbody>

HTML element

**Attributes:**
+ [style](#style-attribute)

**Childs:**
+ [\<tr>](#tr)

***

## \<thead>

HTML element

**Attributes:**
+ [style](#style-attribute)

**Childs:**
+ [\<tr>](#tr)

***

## \<tr>

HTML element

**Attributes:**
+ [style](#style-attribute)

**Childs:**
+ [\<th>](#th)
+ [\<td>](#td)

***

## \<td>

HTML element

**Attributes:**
+ [style](#style-attribute)

**Childs:**
+ [\<div>](#div)
+ [\<hX>](#hX)
+ [\<span>](#span)
+ String literal

***

## \<th>

HTML element, which changes the default formatting (compared to [\<td>](#td))

**Attributes:**
+ [style](#style-attribute)

**Childs:**
+ [\<div>](#div)
+ [\<hX>](#hX)
+ [\<span>](#span)
+ String literal

***

## \<div>

HTML element

**Attributes:**
+ class
+ [style](#style-attribute)

**Childs:**
+ [\<div>](#div)
+ [\<hX>](#hX)
+ [\<span>](#span)
+ [\<style>](#style)
+ [\<table>](#table)
+ String literal

***

## \<style>

HTML element which holds CSS definitions

**Attributes:**

**Childs:**
+ CSS definition(s)

***

## \<span>

HTML element

**Attributes:**

**Childs:**
+ String literal

***

## \<hX>

HTML header element. X can be between 1 and 6

**Attributes:**
+ [\<style>](#style)

**Childs:**
+ String literal

***

# Attributes

<h2 id="style-attribute">style</h2>

Style is based on CSS and defines how the element should be displayed.<br>
Example usage:
```HTML
<element style="property1: value1; property2: value2">
```
**Properties**
+ border
+ color
+ font-family
+ font-size
+ font-weight
+ text-align
+ vertical-align
+ width

***
