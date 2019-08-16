FILES = misc.jemdoc toc_calendar.jemdoc

all: $(FILES)
	python jemdoc.py $(FILES)
	python jemdoc.py -c show_abstract.conf index.jemdoc
	python jemdoc.py -c show_abstract.conf publications_list.jemdoc
	python jemdoc.py -c show_abstract.conf publications.jemdoc
	python jemdoc.py -c show_abstract.conf acseminar.jemdoc
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

publicationslist:
	python jemdoc.py -c show_abstract.conf publications_list.jemdoc
	mv publications_list.html ../.

clean:
	rm -v *~
