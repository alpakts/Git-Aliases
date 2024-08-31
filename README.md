# Git-Aliases
Cheatsheet for git aliases

Languages [EN](#en) | [TR](#tr)
## EN

### Overview

This document provides a comprehensive set of Git aliases designed to streamline your workflow by shortening commonly used Git commands. Aliases are shortcuts that allow you to execute commands more efficiently, saving time and reducing the chances of errors.

### Alias List and Descriptions

| Alias | Git Command | Description |
|-------|-------------|-------------|
| `gl`  | `git pull`  | Fetches and merges changes from the remote repository into the current branch. |
| `gp`  | `git push`  | Pushes the committed changes from the local repository to the remote repository. |
| `gs`  | `git status`| Displays the state of the working directory and staging area. |
| `gb`  | `git branch`| Lists all branches in the repository or creates a new branch. |
| `gco` | `git checkout` | Switches branches or restores working tree files. |
| `gcb` | `git checkout -b` | Creates and switches to a new branch. |
| `gd`  | `git diff`  | Shows the differences between the working directory and the index. |
| `ga`  | `git add`   | Adds file contents to the staging area. |
| `gc`  | `git commit`| Records changes to the repository with a message. |
| `gcm` | `git commit -m` | Commits changes with a concise message. |
| `gr`  | `git rebase` | Reapplies commits on top of another base tip. Useful for integrating changes. |
| `gm`  | `git merge`  | Combines multiple sequences of commits into one unified history. |
| `grh` | `git reset HEAD~` | Resets the current HEAD to the specified state, typically used to undo the last commit. |
| `gst` | `git stash`  | Temporarily stores all modified tracked files. Use `git stash pop` to retrieve them. |
| `glg` | `git log --oneline --graph --all` | Displays a condensed view of the commit history with a graphical representation of branches. |
| `gfa` | `git fetch --all` | Fetches all changes from all remote repositories. |
| `gcl` | `git clone`  | Clones a repository into a new directory. |

### Setting Up Git Aliases

To set up these aliases, follow the instructions based on your operating system:

#### For Git Bash, Linux, and macOS Users:

1. **Open your terminal.**
2. **Navigate to your home directory:**
   ```bash
   cd ~
   ```
3. **Open the `.bashrc` or `.bash_profile` file:**
   ```bash
   nano ~/.bashrc
   ```
   or
   ```bash
   nano ~/.bash_profile
   ```
4. **Append the following aliases to the end of the file:**
   ```bash
   alias gl='git pull'
   alias gp='git push'
   alias gs='git status'
   alias gb='git branch'
   alias gco='git checkout'
   alias gcb='git checkout -b'
   alias gd='git diff'
   alias ga='git add'
   alias gc='git commit'
   alias gcm='git commit -m'
   alias gr='git rebase'
   alias gm='git merge'
   alias grh='git reset HEAD~'
   alias gst='git stash'
   alias glg='git log --oneline --graph --all'
   alias gfa='git fetch --all'
   alias gcl='git clone'
   ```
5. **Save and close the file.**
   - **To save:** Press `Ctrl + O`, then `Enter`
   - **To exit:** Press `Ctrl + X`
6. **Apply the changes by refreshing the shell:**
   ```bash
   source ~/.bashrc
   ```
   or
   ```bash
   source ~/.bash_profile
   ```

#### For Windows PowerShell Users:

1. **Open PowerShell.**
2. **Edit your PowerShell profile file:**
   ```powershell
   notepad $PROFILE
   ```
3. **Add the following alias functions:**
   ```powershell
   Set-Alias gl git-pull
   function git-pull { git pull }

   Set-Alias gp git-push
   function git-push { git push }

   Set-Alias gs git-status
   function git-status { git status }

   Set-Alias gb git-branch
   function git-branch { git branch }

   Set-Alias gco git-checkout
   function git-checkout { git checkout }

   Set-Alias gcb git-checkout-b
   function git-checkout-b { git checkout -b }

   Set-Alias gd git-diff
   function git-diff { git diff }

   Set-Alias ga git-add
   function git-add { git add }

   Set-Alias gc git-commit
   function git-commit { git commit }

   Set-Alias gcm git-commit-m
   function git-commit-m { git commit -m }

   Set-Alias gr git-rebase
   function git-rebase { git rebase }

   Set-Alias gm git-merge
   function git-merge { git merge }

   Set-Alias grh git-reset-head
   function git-reset-head { git reset HEAD~ }

   Set-Alias gst git-stash
   function git-stash { git stash }

   Set-Alias glg git-log-graph
   function git-log-graph { git log --oneline --graph --all }

   Set-Alias gfa git-fetch-all
   function git-fetch-all { git fetch --all }

   Set-Alias gcl git-clone
   function git-clone { git clone }
   ```
4. **Save and close the profile file.**
5. **Activate the changes by restarting PowerShell or running:**
   ```powershell
   . $PROFILE
   ```

### Using Git Aliases

Once configured, you can use the aliases in your terminal to streamline your Git workflow:

- **`gl`**: Equivalent to `git pull`
- **`gp`**: Equivalent to `git push`
- **`gs`**: Equivalent to `git status`
- **`gb`**: Equivalent to `git branch`
- **`gco`**: Equivalent to `git checkout <branch-name>`
- **`gcb`**: Equivalent to `git checkout -b <new-branch-name>`
- **`gd`**: Equivalent to `git diff`
- **`ga`**: Equivalent to `git add <file-name>` or `ga .` (to add all files)
- **`gc`**: Equivalent to `git commit`
- **`gcm`**: Equivalent to `git commit -m "Commit message"`
- **`gr`**: Equivalent to `git rebase`
- **`gm`**: Equivalent to `git merge`
- **`grh`**: Equivalent to `git reset HEAD~`
- **`gst`**: Equivalent to `git stash`
- **`glg`**: Equivalent to `git log --oneline --graph --all`
- **`gfa`**: Equivalent to `git fetch --all`
- **`gcl`**: Equivalent to `git clone <repository-url>`

### Conclusion

Git aliases are powerful shortcuts that help you perform frequent operations more efficiently. By integrating these aliases into your workflow, you can save time and reduce errors, enhancing your productivity in managing Git repositories.


# Git Aliasları

## TR
### Genel Bakış

Bu dökümantasyon, Git komutlarını kısaltarak iş akışınızı hızlandırmanıza yardımcı olacak bir dizi Git alias'ını (kısayol) içermektedir. Alias'lar, komutları daha verimli bir şekilde çalıştırmanıza olanak tanıyan kısa yollardır.

### Alias Listesi ve Açıklamaları

| Alias | Git Komutu | Açıklama |
|-------|------------|----------|
| `gl`  | `git pull`  | Uzak depodaki değişiklikleri çekip mevcut dala entegre eder. |
| `gp`  | `git push`  | Yerel depodaki değişiklikleri uzak depoya gönderir. |
| `gs`  | `git status`| Çalışma dizini ve hazırlık alanındaki durumu gösterir. |
| `gb`  | `git branch`| Depodaki tüm dalları listeler veya yeni bir dal oluşturur. |
| `gco` | `git checkout` | Dallar arasında geçiş yapar veya çalışma dizinindeki dosyaları geri yükler. |
| `gcb` | `git checkout -b` | Yeni bir dal oluşturur ve bu dala geçiş yapar. |
| `gd`  | `git diff`  | Çalışma dizini ile index arasındaki farkları gösterir. |
| `ga`  | `git add`   | Dosya içeriklerini hazırlık alanına ekler. |
| `gc`  | `git commit`| Değişiklikleri mesaj ile birlikte depoya kaydeder. |
| `gcm` | `git commit -m` | Değişiklikleri kısa bir mesaj ile kaydeder. |
| `gr`  | `git rebase` | Commit'leri başka bir temel uç üzerinde yeniden uygular. Değişiklikleri entegre etmek için kullanışlıdır. |
| `gm`  | `git merge`  | Birden fazla commit dizisini tek bir geçmişte birleştirir. |
| `grh` | `git reset HEAD~` | Mevcut HEAD'i belirtilen duruma sıfırlar, genellikle son commit'i geri almak için kullanılır. |
| `gst` | `git stash`  | Tüm değişiklikleri geçici olarak saklar. `git stash pop` komutuyla geri alınabilir. |
| `glg` | `git log --oneline --graph --all` | Dalların grafiksel bir temsili ile commit geçmişini gösterir. |
| `gfa` | `git fetch --all` | Tüm uzak depolardan değişiklikleri alır. |
| `gcl` | `git clone`  | Bir depoyu yeni bir dizine klonlar. |

### Git Alias'larının Kurulumu

Bu alias'ları kurmak için işletim sisteminize göre aşağıdaki adımları takip edin:

#### Git Bash, Linux ve macOS Kullanıcıları:

1. **Terminalinizi açın.**
2. **Ana dizine gidin:**
   ```bash
   cd ~
   ```
3. **`.bashrc` veya `.bash_profile` dosyanızı açın:**
   ```bash
   nano ~/.bashrc
   ```
   veya
   ```bash
   nano ~/.bash_profile
   ```
4. **Alias'ları dosyanın sonuna ekleyin:**
   ```bash
   alias gl='git pull'
   alias gp='git push'
   alias gs='git status'
   alias gb='git branch'
   alias gco='git checkout'
   alias gcb='git checkout -b'
   alias gd='git diff'
   alias ga='git add'
   alias gc='git commit'
   alias gcm='git commit -m'
   alias gr='git rebase'
   alias gm='git merge'
   alias grh='git reset HEAD~'
   alias gst='git stash'
   alias glg='git log --oneline --graph --all'
   alias gfa='git fetch --all'
   alias gcl='git clone'
   ```
5. **Dosyayı kaydedin ve kapatın.**
   - **Kaydetmek için:** `Ctrl + O`, ardından `Enter`
   - **Çıkmak için:** `Ctrl + X`
6. **Değişiklikleri uygulayın:**
   ```bash
   source ~/.bashrc
   ```
   veya
   ```bash
   source ~/.bash_profile
   ```

#### Windows PowerShell Kullanıcıları:

1. **PowerShell'i açın.**
2. **PowerShell profil dosyanızı açın:**
   ```powershell
   notepad $PROFILE
   ```
3. **Profil dosyanıza aşağıdaki alias fonksiyonlarını ekleyin:**
   ```powershell
   Set-Alias gl git-pull
   function git-pull { git pull }

   Set-Alias gp git-push
   function git-push { git push }

   Set-Alias gs git-status
   function git-status { git status }

   Set-Alias gb git-branch
   function git-branch { git branch }

   Set-Alias gco git-checkout
   function git-checkout { git checkout }

   Set-Alias gcb git-checkout-b
   function git-checkout-b { git checkout -b }

   Set-Alias gd git-diff
   function git-diff { git diff }

   Set-Alias ga git-add
   function git-add { git add }

   Set-Alias gc git-commit
   function git-commit { git commit }

   Set-Alias gcm git-commit-m
   function git-commit-m { git commit -m }

   Set-Alias gr git-rebase
   function git-rebase { git rebase }

   Set-Alias gm git-merge
   function git-merge { git merge }

   Set-Alias grh git-reset-head
   function git-reset-head { git reset HEAD~ }

   Set-Alias gst git-stash
   function git-stash { git stash }

   Set-Alias glg git-log-graph
   function git-log-graph { git log --oneline --graph --all }

   Set-Alias gfa git-fetch-all
   function git-fetch-all { git fetch --all }

   Set-Alias gcl git-clone
   function git-clone { git clone }
   ```
4. **Dosyayı kaydedin ve kapatın.**
5. **Değişikliklerin uygulanması için PowerShell'i yeniden başlatın veya şu komutu çalıştırın:**
   ```powershell
   . $PROFILE
   ```

### Git Alias'larını Kullanma

Alias'lar yapılandırıldıktan sonra, terminalde bu kısa yolları kullanarak Git iş akışınızı hızlandırabilirsiniz:

- **`gl`**: `git pull` komutunun kısa yolu.
- **`gp`**: `git push` komutunun kısa yolu.
- **`gs`**: `git status` komutunun kısa yolu.
- **`gb`**: `git branch` komutunun kısa yolu.
- **`gco`**: `git checkout <branch-name>` komutunun kısa yolu.
- **`gcb`**: `git checkout -b <new-branch-name>` komutunun kısa yolu.
- **`gd`**: `git diff` komutunun kısa yolu.
- **`ga`**: `git add <file-name>` komutunun kısa yolu veya tüm dosyalar için `ga .`
- **`gc`**: `git commit` komutunun kısa yolu.
- **`gcm`**: `git commit -m "Commit message"` komutunun kısa yolu.
- **`gr`**: `git rebase` komutunun kısa yolu.
- **`gm`**: `git merge` komutunun kısa yolu.
- **`grh`**: `git reset HEAD~` komutunun kısa yolu.
- **`gst`**: `git stash` komutunun kısa yolu.
- **`glg`**: `git log --oneline --graph --all` komutunun kısa yolu.
- **`gfa`**: `git fetch --all` komutunun kısa yolu.
- **`gcl`**: `git clone <repository-url>` komutunun kısa yolu.

### Sonuç

Git alias'ları, sık kullanılan işlemleri daha verimli bir şekilde gerçekleştirmenize yardımcı olan güçlü kısa yollardır. Bu alias'ları iş akışınıza entegre ederek, zaman kazanabilir ve hataları azaltabilir, Git depolarını yönetme verimliliğinizi artırabilirsiniz.

