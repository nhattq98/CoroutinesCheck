# CoroutinesCheck

**1. Every Coroutines needs to be started in a logical scope with a limited lifetime** \n
**2. Coroutine started in the same scope from a hierarchy** \n
**3. Parent Job won't be completed until all of its children have completed** \n
**4. Canceling a parent will cancel all children, canceling a child won't cancel the parent or siblings** \n
**5. If a child fails, the exception is propagated upwards and depending on the job type, either all siblings are canceled or note** \n
