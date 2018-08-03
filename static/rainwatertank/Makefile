all: desk_distances.html tank_distances.html tank_broken_distances.html

# desk_distances.html: desk_distances.ipynb desk_distances.txt
# 	jupyter nbconvert --to html desk_distances.ipynb

# tank_distances.html: tank_distances.ipynb tank_distances.txt
# 	jupyter nbconvert --to html tank_distances.ipynb

# tank_broken_distances.html: tank_broken_distances.ipynb tank_broken_distances.txt
# 	jupyter nbconvert --to html tank_broken_distances.ipynb

%.html: %.ipynb %.txt
	jupyter nbconvert --to html $(patsubst %.html,%.ipynb,$@)

clean:
	rm *.html