## gitlab-irc

Provides IRC notifications for GitLab repositories. Built with Sinatra and cinch. Uses GitLab's web hooks, no voodoo required.

Example:

> [gitlab-irc(master)] nTraum | initial commit | [http://goo.gl/yYTGcM](http://goo.gl/yYTGcM)
### Requirements

* Redis (already installed if you run it on the same host as GitLab)
* Ruby 2.0 (older versions may work as well)
* tmux / screen

### Installation & Usage

1. Clone the repository: `git clone https://github.com/nTraum/gitlab-irc.git`
2. Install gems: `cd gitlab-irc; bundle`
2. Edit `config/config.yml` to your needs
3. Start the app: `foreman start` in a tmux / screen shell
4. Add a web hook pointing to the app: `http://localhost/commit:4567` (host / port may differ, depending on your configuration)

### License

[WTFPL](http://www.wtfpl.net/txt/copying/)
