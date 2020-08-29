Ansible playbook for creating a Jekyll Scaffold with Bundler.

[MORE ABOUT USING JEKYLL WITH BUNDLER](https://masya.github.io/other/2020/08/20/github-jekyll-part-02.html)

Tested on Vagrant ubuntu/bionic64, Ansible 2.9.11.

### Installation
1) Prepare vagrant environment

2) Run:
```sh
ansible-playbook jekyll.yml 
```

### Advanced
1) needed fixes for static versions
- jekyll_version
- ruby_version
[Github Pages - Dependency versions](https://pages.github.com/versions/)
Get versions from page dinamically.

2) install jekyll with bundler
- shell
Сreate a module with errors and result handling.
