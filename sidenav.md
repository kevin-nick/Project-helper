# Sidenav

## Font awesome link

```html
<link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css"
    integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p" crossorigin="anonymous" />
```

## styles.scss

```scss
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    position: relative;
    font-family: 'Roboto', sans-serif;
}

.card {
    display: flex;
    flex-direction: column;
    border-radius: .5rem;
    background-color: #fff;
    margin: 1.25rem 0 1.25rem 0;
    box-shadow: 0 .25rem .5rem #e6edef;

    .card-head {
        padding: 1rem 1.5rem;
        border-bottom: 1px solid #edf1f7;
        font-size: 1rem;
        font-weight: 600;
    }

    .card-body {
        padding: 1rem 1.5rem; 
    }
}
```
## styles.scss

```scss sidenav

.sidenav {
    background-color: rgb(0, 119, 255);
    transition: all .5s ease;
    position: fixed;
    top: 0;
    z-index: 1;
    width: 5rem;
    height: 100vh;
    box-shadow: 0.063rem 0 1.25rem 0 #8990a3;
    .logo-container {
        display: flex;
        align-items: center;
        padding: 0.938rem 0.938rem 0 0.938rem;
        width: 100%;
        .logo {
            background: #fff;
            text-align: center;
            width: 3rem;
            min-width: 3rem;
            padding: 0.313rem;
            border-radius: 0.313rem;
            font-size: 24px;
            font-weight: 900;
            cursor: pointer;
            border: none;
        }
        .logo-text {
            margin-left: 1.5rem;
            font-size: 24px;
            font-weight: 700;
            color: #fff;
        }
        .Btn-close {
            margin-left: auto;
            cursor: pointer;
            width: 2rem;
            height: 2rem;
            border-radius: 50%;
            background: transparent;
            border: none;
            .fa-times {
                color: #fff;
                font-size: 24px;
            }
        }
    }
}

.sidenav-collapsed {
    width: 14rem;
}

.sidenav-nav {
    list-style: none;
    padding: 0938rem;
    margin: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    height: calc(100% - 3.65rem);
    cursor: pointer;
    .sidenav-nav-item {
        width: 100%;
        margin-bottom: 0.625rem;
        .sidenav-nav-link {
            display: flex;
            align-items: center;
            height: 3rem;
            color: #f3f3f3;
            text-decoration: none;
            transition: all .3s ease;
            .sidenav-link-icon {
                font-size: 22px;
                width: 2rem;
                min-width: 2rem;
                margin: 0 0.5rem;
                text-align: center;
            }
            .sidenav-link-text {
                margin-left: 1.5rem;
                color: #fff;
            }
        }
    }
}
```

## Commands used

To generate components : 

`ng g c body --skip-tests true` 

`ng g c sidenav --skip-tests true` 

`ng g c dashboard --skip-tests true` 

`ng g c products --skip-tests true` 

`ng g c statistics --skip-tests true` 

`ng g c coupens --skip-tests true` 

`ng g c pages --skip-tests true` 

`ng g c media --skip-tests true` 

`ng g c settings --skip-tests true` 
