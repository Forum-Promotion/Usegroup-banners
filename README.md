# Usegroup-banners

In extra.css, the contents are

```
.usergroup-banner {
    position: relative;
    padding: 1.8px;
    margin: 3px;
    display: block;
    width: 100%;
}
.usergroup-image {
    display: inline-block;
    width: 10%;
}
.usergroup-text strong {
    background: #222;
	width: 100%;
    font-weight: bold;
    text-align: center;
    display: inline-block;
	color: white;
	padding-top: 1px;
}
.admin {
    background: linear-gradient(to right, #105da5, #2877fb);
}
.ct {
    background: linear-gradient(to right, #105da5, #49891e);
}
.pt {
    background: linear-gradient(to right, #105da5, #FF0000);
}
.mt {
    background: linear-gradient(to right, #105da5, #f7acbb);
}
.rt {
    background: linear-gradient(to right, #105da5, #990033);
}
.gt {
    background: linear-gradient(to right, #105da5, #E2703A);
}
.et {
    background: linear-gradient(to right, #105da5, #5f9ea0);
}

```

To add another team banner, paste this code snippet below the code above and modify the class `<team>` to the desired team e.g. `.devs`.

```
.<team> {
    background: linear-gradient(to right, #105da5, <team-color>);
}
```

Under usergroup settings and user banner styling using `Other, using custom CSS class name`. The following is entered:

```
    usergroup-banner usergroup-text username-span <team>
```

Modify <team> to the class created in extra.css.

Save and review site to ensure banner is applied.
