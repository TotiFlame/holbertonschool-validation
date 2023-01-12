build: ## Generate the website from the markdown and configuration files in the directory
	hugo > /dev/null 2>&1
clean: ## Cleanup the content of the directory dist/
	rm -r dist/*
post: ## Create a new blog post whose filename and title come from the environment variables POST_TITLE and POST_NAME
	hugo new posts/$(POST_NAME).md ; sed -i 's/title:.*/title: "$(POST_TITLE)"/' content/posts/$(POST_NAME).md
help: ## Show help
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'
hello: ## Display hello
	echo "hello"
package: ## Create the zip file
	zip -r awesome-website.zip awesome-api dist/
lint: ## Update to lint the files README.md and DEPLOY.md with markdownlint command line
	markdownlint --fix README.md DEPLOY.md