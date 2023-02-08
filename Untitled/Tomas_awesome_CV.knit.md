---
name: Tomas
surname: Quezada
position: Entomology Technician
address: Cornell University
phone: +1 956-286-1840
email: TAQ3@cornell.edu
github: https://github.com/taq42408
date: February 2023
output:
  vitae::awesomecv:
    page_total: yes
nocite: '@R-vitae, @R-tibble'
csl: /Library/Frameworks/R.framework/Versions/4.2/Resources/library/vitae/vitae.csl

---

```r
readExcelSheets <- function(filename){
  # read all sheets in .xlsx 
  all <- readxl::excel_sheets(filename)
  
  # import each sheet into a list using readxl::read_excel
  list <- lapply(all, function(x) readxl::read_excel(filename, sheet = x))
  
  # save sheet name for each sheet (list)
  names(list) <- all
  
  # breaks up list and creates a dataframe for each sheet with df names matching sheet names
  list2env(list, envir = .GlobalEnv)
}
```





# Some stuff about me

 * I poisoned myself doing research.
 * I was the first woman to win a Nobel prize
 * I was the first person and only woman to win a Nobel prize in two different sciences.

# Education

\begin{cventries}
	\cventry{Informal studies}{Flying University}{Warsaw, Poland}{1889-91}{}\vspace{-4.0mm}
	\cventry{Master of Physics}{Sorbonne Université}{Paris, France}{1893}{}\vspace{-4.0mm}
	\cventry{Master of Mathematics}{Sorbonne Université}{Paris, France}{1894}{}\vspace{-4.0mm}
\end{cventries}

# Nobel Prizes

\begin{cvhonors}
	\cvhonor{}{Nobel Prize in Physics}{Awarded for her work on radioactivity with Pierre Curie and Henri Becquerel}{1903}
	\cvhonor{}{Nobel Prize in Chemistry}{Awarded for the discovery of radium and polonium}{1911}
\end{cvhonors}

# Publications


::: {#bibliography}
/var/folders/5z/2hvg1nk9689fqfgq_tgx0w8w0000gp/T//RtmpRu9iaf/file3c1917a31930.yaml
:::

