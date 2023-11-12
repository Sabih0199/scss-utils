# Scss Utils

## Authors

- [@Sabih0199](https://www.github.com/Sabih0199)


## 🛠 Skills
SCSS...


# Hi, I'm Sabih! 👋


## 🚀 About Me
I'm a creative ui developer...


## Authors

- [@Sabih0199](https://www.github.com/Sabih0199)


## Usage/Examples

Download or copy file code and create a file with .scss ext*

Prepend utils.scss file in your project config e.g vite.config, next.config

```javascript
-- vite config
 css: {
        preprocessorOptions: {
            scss: {
                additionalData: `
            @import "url to file";
          `
            }
        }
    }

-- next config
 sassOptions: {
        prependData: `@import "url to file";`
    }
```

Now, you can use predefined $variables, functions or mixins written in this file. You don't need import statements in any other scss file to use variables, mixings or functions.

```scss
==> This will generate my-fs-0 to my-fs-50 in em unit

@include generateUtilClass("my-fs", "font-size");

==> Same you can create custom classess ranging from my-width-0 to my-width-250 (ofcourse you can modify max limit... :))

@include generateUtilClass("my-width-w", "width");

@include generateUtilClass("your-prefix-h", "height");

@include generateUtilClass("your-prefix-pr", "padding-right");

@include generateUtilClass("your-prefix-pl", "padding-left");

==>All margins will be generated in rem unit if third args `true`

@include generateUtilClass("your-prefix-mb", "margin-block-end", 
true);
```

Still need help? Reach me through my email sabihali1k99@gmail.com 
