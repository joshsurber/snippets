
``` css
/* Bleed full element */  
.full-bleed {  
	margin: 0 calc(50% - 50vw);  
}  
  
/* Bleed background color only */  
.full-bleed {  
	box-shadow: 0 0 0 100vmax var(--clr-bg);  
	clip-path: inset(0 -100vmax);  
}
```