FILES = index.jemdoc misc.jemdoc

all: $(FILES)
	python2 jemdoc.py $(FILES)
	python2 jemdoc.py -c show_abstract.conf publications.jemdoc
	mv *.html ../.

index:
	python2 jemdoc.py -c show_abstract.conf index.jemdoc
	mv index.html ../.

acseminar:
	python2 jemdoc.py -c show_abstract.conf acseminar.jemdoc
	mv acseminar.html ../.

publications:
	python2 jemdoc.py -c show_abstract.conf publications.jemdoc
	mv publications.html ../.

publicationstopic:
	python2 jemdoc.py -c show_abstract.conf publications_topic.jemdoc
	mv publications_topic.html ../.

toccalendar:
	python2 jemdoc.py toc_calendar.jemdoc
	mv toc_calendar.html ../.

clean:
	rm -v *~
