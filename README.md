## Goal: 
Build an autonomous Dev team that generates, reviews, tests, fixes, and reports on the Python code using a LangGrap controlled workflow.

## Entire workflow

        User
          | requirement prompt
        Initial state
            |
        Developer node
        Generate py code
            |
   (A) ---Reviewer node
        LLM will review against the best practices
            |
           QA node
            |
           QA router
           needs_fix = Yes/No
          /           \
        Yes            No
        /               \
      Fix               Report
      Improve code          |
        |                   END
       (A)

### NODES:
1. Developer
2. Reviewer
3. QA
4. Fixer
5. Reporter
6. Router