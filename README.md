# Rename your `main` branch to `master`

Recently, GitHub decided to name the default branch upon new repository creation to `main`, in response to... diversity or social justice or blah blah blah.
I won't go over why I think this is a stupid idea - that has been covered exhaustively in a million threads on Twitter, Reddit, GitHub itself, etc. - but suffice to say, I don't like it.
So I wrote this little script to convert everything back to the way it should be:

```sh
./main2master user/repo PAT
```

This will make a `master` branch from your existing `main`, push the former up, and delete the latter.
An easy way to restore sanity if your overly woke colleagues or collaborators got a little bit too excited about the power of version control to... end racism.. or something.

**To do:**

- Replicate branch protection in the new `master`.
- Figure out how to do the deletion without a PAT.
