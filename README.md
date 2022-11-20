```py
from github import Profile, you
prof = Profile("Welcome To LineLib!")

@prof.when('view', user=you)
def when_you_see_this(event):
  event.profile.show()
  
prof.run_until('destroyed')
```
