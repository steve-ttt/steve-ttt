# 👨‍💻 Stephen T

```scheme
;; profile.scm
(define me
  '((name      . "Steve T")
    ;; List of lists: ((Title Status) ...)
    (roles     . (("Linux Specialist" "Full Time")
                  ("Master's Student" "Part Time")))                  
    (languages . (Go C Scheme C++ Python Java))
    (editor    . ("Emacs" "Neovim" "VSCode"))))

(define (introduce user)
  (format #t "Hi! I'm ~a.\n" (cdr (assoc 'name user)))
  (display "Current Status:\n")
  ;; Iterate over the list of lists using a Lambda
  (for-each (lambda (job)
              (format #t " * ~a (~a)\n" (car job) (cadr job)))
            (cdr (assoc 'roles user)))
  (format #t "I code in: ~a\n" (cdr (assoc 'languages user)))
  (format #t "I edit with: ~a\n" (cdr (assoc 'editor user))))

;; Execute
(introduce me)


### 🛠️ Tech Stack
<p align="left"> <img src="https://skillicons.dev/icons?i=go,c,cpp,clojure,python,emacs,vim,neovim,linux,git" /> </a> </p>

### ☕ About Me
- 🔭 I'm Steve, a passionate computer scientist and Linux specialist working full-time while pursuing my Master's degree in Computer Science part-time. 
- 🌱 I’m currently pursuing my Master's  Masters of Science in Computer Science
- 👯 I’m looking to Build / collaborate on a Compiler design for Scheme/LISP

