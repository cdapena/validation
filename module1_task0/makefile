.POSIX:
DESTDIR=dist/public
HUGO_VERSION=0.58.3

.HUGO: all
all: clean build post 

.HUGO: clean
clean:
	@echo "? Cleaning old build"
	cd $(DESTDIR) && rm -rf *

.HUGO: build
build:
	@echo "? Generating site"
	hugo --gc -d $(DESTDIR)

.HUGO: post 
test:
	@echo "? Posting"
	touch dist/content/posts/$POST_NAME
	echo "titl
> $POST_TITLE
