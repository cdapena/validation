.POSIX:
DESTDIR=public
DESTDIRPOST=content/posts/


.HUGO: all
all: clean build post 

.HUGO: clean
clean:
	@echo "Cleaning old build"
	@cd $(DESTDIR) && rm -rf *

.HUGO: build
build:
	@echo "Generating site"
	@hugo -d $(DESTDIR)

.HUGO: post
post:
	@echo "Posting"
	@echo title: $(POST_TITLE) > content/posts/$(POST_NAME)


