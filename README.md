```bash
cd /opt/instana/agent/etc/instana
git init
echo '*' > .gitignore
echo '!com.instana.agent.bootstrap.AgentBootstrap.cfg' >> .gitignore
git add .gitignore
git add com.instana.agent.bootstrap.AgentBootstrap.cfg
git commit -m "Add only the specified config file to the repository"
git remote add origin git@github.com:kdrkrst/version-only-agent-config-repo-linux.git
git branch -M main
git push -u origin main
```

+ ci/cd automation
	pull hook
	reboot agent | UpdateManager config
	
	
