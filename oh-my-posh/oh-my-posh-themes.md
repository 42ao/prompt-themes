# Oh-my-posh prompt templates
Oh my posh is a "prompt theme engine for any shell". See also [ohmyposh.dev](https://ohmyposh.dev/).

In the following, I describe the idea behind my personal themes.

## pure-42ao
* based on `pure` profile
* puristic focussing on essential information
* contains
    - full path
        - in <span style="color:lightblue">light blue</span> just like folders listed via the bash `ls` command
    - git branch (if available)
        - in <span style="color:#F34C27">"git" orange</span>
        - with upstream icon
    - git status (if available)
        - <span style="color:green">repo ok</span>
        - <span style="color:yellow">repo modified</span>
        - <span style="color:cyan">#commits ahead</span>
        - <span style="color:magenta">#commits behind</span>
        - <span style="color:red">diverged: #commits ahead and behind</span>
        - <span style="color:red">#files in workspace</span>
            - `+` untracked files
        - <span style="color:green">#files in index / staged</span>
            - `+` added
            - `~` modified
            - `-` deleted
        - <span style="color:yellow">#stashes</span>
        - <span style="color:gray">#worktrees</span>
    - execution time of last command
        - right aligned so that execution times can be easily compared
    - prompt
        - prompt color indicates state of last execution: <span style="color:green">ok</span> or <span style="color:red">failed</span>
        - in separate row so that commands are always aligned
