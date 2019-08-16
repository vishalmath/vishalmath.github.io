FILES = misc.jemdoc toc_calendar.jemdoc

all: $(FILES)
	python jemdoc.py $(FILES)
	python jemdoc.py -c show_abstract.conf index.jemdoc
	python jemdoc.py -c show_abstract.conf publications_list.jemdoc
	python jemdoc.py -c show_abstract.conf publications.jemdoc
	python jemdoc.py -c show_abstract.conf acseminar.jemdoc

index:
	python jemdoc.py -c show_abstract.conf index.jemdoc

acseminar:
	python jemdoc.py -c show_abstract.conf acseminar.jemdoc

publications:
	python jemdoc.py -c show_abstract.conf publications.jemdoc

publicationslist:
	python jemdoc.py -c show_abstract.conf publications_list.jemdoc

clean:
	rm -v *~
