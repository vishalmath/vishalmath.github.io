FILES = index.jemdoc misc.jemdoc

all: $(FILES)
	python jemdoc.py $(FILES)
	python jemdoc.py -c show_abstract.conf publications.jemdoc
	mv *.html ../.

index:
	python jemdoc.py -c show_abstract.conf index.jemdoc
	mv index.html ../.

acseminar:
	python jemdoc.py -c show_abstract.conf acseminar.jemdoc
	mv acseminar.html ../.

publications:
	python jemdoc.py -c show_abstract.conf publications.jemdoc
	mv publications.html ../.

publicationstopic:
	python jemdoc.py -c show_abstract.conf publications_topic.jemdoc
	mv publications_topic.html ../.

toccalendar:
	python jemdoc.py toc_calendar.jemdoc
	mv toc_calendar.html ../.

clean:
	rm -v *~
