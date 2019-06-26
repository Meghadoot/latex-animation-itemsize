# latex-animation-itemsize
This repository presents possible examples to animate presentation slides with Itemize or Enumerate List.



### Using `\uncover`

  ```
\documentclass{beamer}
\begin{document}
\begin{frame}
\begin{enumerate}
\uncover<1->{\item Hi}
\uncover<2->{\item Hello}
\uncover<3->{\item Hi again}
\uncover<4->{\item Hello again}
\end{enumerate}
\end{frame}
\end{document}
   ```
![8R35O](https://user-images.githubusercontent.com/25079922/60218315-3df88600-986f-11e9-8fca-83ebec5a9a1c.gif)


### Using `\only`

  ```
\documentclass{beamer}
\begin{document}
\begin{frame}
\begin{enumerate}
\only<1->{\item Hi}
\only<2->{\item Hello}
\only<3>{\item Hi again}   %% note absence of - after 3
\only<4->{\item Hello again}
\end{enumerate}
\end{frame}
\end{document}
   ```
  
![RntlP](https://user-images.githubusercontent.com/25079922/60219686-b2cdbf00-9873-11e9-8b70-5682a55b79ed.gif)



### Using `overlayarea`

  ```
\documentclass{beamer}
\begin{document}
\begin{frame}
\begin{overlayarea}{\textwidth}{.5\textheight}
\begin{enumerate}
\only<1->{\item Hi}
\only<2->{\item Hello}
\only<3>{\item Hi again}   %% note absence of - after 3
\only<4->{\item Hello again}
\end{enumerate}
\end{overlayarea}
\end{frame}
\end{document}
   ```
 ![2KNhf](https://user-images.githubusercontent.com/25079922/60220039-fffe6080-9874-11e9-9626-6ac2f2d7f09b.gif)


  ### Using `\pause`

  ```
\documentclass{beamer}
\begin{document}
\begin{frame}
\begin{enumerate}
\item Hi \pause
\item Hello \pause
\item Hi again \pause
\item Hello again 
\end{enumerate}
\end{frame}
\end{document}
   ```
  ![bjJXf](https://user-images.githubusercontent.com/25079922/60220575-c6c6f000-9876-11e9-903b-a394d6414890.gif)


### Only one item per slide
   
  ```
\documentclass{beamer}
\begin{document}
\begin{frame}
\begin{enumerate}
\item<1> Hi 
\item<2> Hello 
\item<3> Hi again 
\item<4> Hello again
\end{enumerate}
\end{frame}
\end{document}
   ```
 ![BWaKr](https://user-images.githubusercontent.com/25079922/60220674-26bd9680-9877-11e9-99a2-25df0ddfe86a.gif)
  



