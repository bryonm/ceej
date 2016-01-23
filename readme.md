# Ceej

Ceej is a set of simple, colorful HTML email templates geared towards account management. It follows the Litmus Template Guidelines and features a full set of templates for damned near any approach to email marketing: traditional responsive, mobile-first, and hybrid, too. 

# Litmus Template Guidelines

## Basic Requirements

- CSS must be inlined
- Base width 600px (for hybrid/spongy + traditional responsive)
- Use media queries starting at 600px - use multiple if necessary
- For traditional responsive, use fixed width of 600px for table structure then optimize w/ media queries
- Mobile-aware base width 480px
- Use media queries starting at 480px
- Email structure must have parent table that wraps every module in its own table row/cell
- No empty cells or spacer gifs - use padding on table cells (exception of empty cells for some hybrid/spongy)
- Use semantic text tags <h1> <p>
- Include View in browser, unsubscribe, address links
- Traditional responsive - fixed table w/ media queries
- Base 14px text
- Buttons need to be tappable - minimum 12px padding around text link
- Must render in all available Litmus clients


## Doctype

```
<!doctype html>
```

## HTML / Head tags (plain)

```
<html>
<head>
```

## Title (empty)

```
<title></title>
```

## Meta tags

```
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<meta http-equiv="X-UA-Compatible" content="IE=edge" />
```

## Reset CSS styles
    
```
body, table, td, a{-webkit-text-size-adjust: 100%; -ms-text-size-adjust: 100%;}
table, td{mso-table-lspace: 0pt; mso-table-rspace: 0pt;}
img{border: 0; height: auto; line-height: 100%; outline: none; text-decoration: none; -ms-interpolation-mode: bicubic;}
table{border-collapse: collapse !important;}
body{height: 100% !important; margin: 0 !important; padding: 0 !important; width: 100% !important;}

a[x-apple-data-detectors] {
    color: inherit !important;
    text-decoration: none !important;
    font-size: inherit !important;
    font-family: inherit !important;
    font-weight: inherit !important;
    line-height: inherit !important;
}
```

## Android 4.4 hack - Insert at bottom of <style>

```
div[style*="margin: 16px 0;"] { margin:0 !important; }
```

## Body

```
<body style=”margin: 0; padding: 0;”>
```

## Hidden Preheader Text

```
<div style="display: none; font-size: 1px; line-height: 1px; max-height: 0px; max-width: 0px; opacity: 0; overflow: hidden;">
    Insert preheader text here.
</div>
```

## MSO Comments

```
<!--[if (gte mso 9)|(IE)]>
```

## Buttons

If solid color, use padding+border-based approach:

```
<table width="100%" border="0" cellspacing="0" cellpadding="0">
  <tr>
    <td>
      <table border="0" cellspacing="0" cellpadding="0">
        <tr>
          <td align="center" style="-webkit-border-radius: 3px; -moz-border-radius: 3px; border-radius: 3px;" bgcolor="#e9703e"><a href="https://litmus.com" target="_blank" style="font-size: 16px; font-family: Helvetica, Arial, sans-serif; color: #ffffff; text-decoration: none; text-decoration: none; border-radius: 3px; padding: 12px 18px; border: 1px solid #e9703e; display: inline-block;">I am a button &rarr;</a></td>
        </tr>
      </table>
    </td>
  </tr>
</table>
```

If gradient or background image, use [VML approach](http://buttons.cm).

## Links

Link to litmus.com

```
<a href=”http://litmus.com” target=”_blank” style=”color: {color};”> </a>
```

## Images

```
<img src=”#” alt=”Alt Text” style=”color: {color}; font-size: {font-size}; display: block; border: 0px;”>
```

## Background Images 

Use backgrounds.cm approach if used.

## Web Fonts

If using @font-face, then wrap in `@media { }` or `@import` as normal.


## Hybrid/Spongy Modules

Here are the hybrid modules to work off of (based off Fabio’s code w/ some slight modifications):

- [1 column](https://litmus.com/builder/148442f)
- [2 column](https://litmus.com/builder/a0db300)
- [2 column w/ gutter](https://litmus.com/builder/7b2d8c6)
- [2 column reverse stack](https://litmus.com/builder/d571f51)
- [2 column reverse stack (w/ gutter)](https://litmus.com/builder/0972fe6)
- [2 column unequal widths](https://litmus.com/builder/4f7c47e)
- [2 column reverse stack (unequal widths)](https://litmus.com/builder/962671d) 
- [3 column](https://litmus.com/builder/896556a)
- [3 column w/ gutter](https://litmus.com/builder/56bce2f)
- [3 column reverse stack](https://litmus.com/builder/bcee4f2)
- [3 columns reverse stack w/ gutter](https://litmus.com/builder/a041970)
- [4 column](https://litmus.com/builder/c02b913)  


## Slate Example

Here are the hybrid/spongy coding guidelines in action with our Slate collection of templates:

- [Newsletter](https://litmus.com/builder/c43272f)
- [Plain](https://litmus.com/builder/4beac75)
- [Product Update](https://litmus.com/builder/e3787c1)
- [Receipt](https://litmus.com/builder/47b218d)
- [Simple Announcement](https://litmus.com/builder/ff595eb)




