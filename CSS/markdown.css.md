#css #md
https://gist.github.com/ImJasonH/c00cdd7aece6945fb8ea
``` css
* {  
	font-size: 12pt;  
	font-family: monospace;  
	font-weight: normal;  
	font-style: normal;  
	text-decoration: none;  
	color: black;  
	cursor: default;  
}  
  
h1::before { content: "# "; }  
h2::before { content: "## "; }  
h3::before { content: "### "; }  
h4::before { content: "#### "; }  
h5::before { content: "##### "; }  
h6::before { content: "###### "; }  
strike::after, strike::before { content: "~~"; }  
i::before, i::after { content: "*"; }  
b::before, b::after { content: "**"; }  
ol, ul { list-style: none; padding-left: 0; }  
ul li::before { content: "* "; }  
ol li::before { content: "1. "; }  
code::before, code::after { content: "`"; }  
pre::before { content: "```" attr(lang) "\A"; }  
pre::after { content:"```\A"; }  
a::before { content: "["; }  
a::after { content: "](" attr(href) ")"; }  
tr::before { content: "| "; }  
td::after { content: " | "; }  
thead td::after { content: " | \A-----| "; white-space: pre; }
```