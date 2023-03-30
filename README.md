![Responsive](https://img.shields.io/badge/Responsive-Yes-ff69b4)
![Bootstrap](https://img.shields.io/badge/bootstrap-5.2.3-blue)

# Form validation w/no JS
For those UI devs who don't touch JS at all, here is a simply HTML and CSS validation, using the pattern attribute and style.

# CSS style validation 

This classes will add the invalid field to the input

```css
    .error-msg{
        display: none;
    }

    input:not(:focus):invalid ~ .error-msg{
        display: block;
    }

    input:not(:focus):invalid{
        border-color: #cb648c;
    }
```

# Config parameters

Also for this to work properly, you need to use the pattern attribute, we're using simple Regex for this example, but you can use a complex Regex for a better validation.

```html
    <input type="text" class="form-control" id="inputAddress2" placeholder="Apartment, studio, or floor" pattern="[A-Za-z]{5,25}">
```
This <DIV> beneath the input is the invalid alert of an incorrect input field

```html
    <input type="text" class="form-control" id="inputAddress2" placeholder="Apartment, studio, or floor" pattern="[A-Za-z]{5,25}">
    <div class="error-msg col-md-6">
        Fill address, more than 5 letters 
    </div>
```

## Libraries included
* Bootstrap v5.2.3
* Jquery v3.5.1

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b your-branch`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin your-branch`
5. Submit a PR

## Creator
* <a href="https://github.com/adhirsaurio">Yomerengues</a>

## Maintenance
![Maintenance](https://img.shields.io/badge/Maintenance-Yes-brightgreen)