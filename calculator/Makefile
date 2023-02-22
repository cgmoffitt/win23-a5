objects = main.o addition.o division.o multiplication.o subtraction.o 

calculator: $(objects)
	cc -o calculator $^

$(objects): %.o:%.c operations.h
	cc -c $< -o $@

clean:
	rm *.o calculator

.PHONY: clean