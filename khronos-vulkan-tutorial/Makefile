INCLUDE_DIR = include/
CFLAGS = -std=c++17 -O3 -I$(INCLUDE_DIR)
LDFLAGS = -lglfw -lvulkan -ldl -lpthread -lX11 -lXxf86vm -lXrandr -lXi

VulkanTest: main.cpp
	g++ $(CFLAGS) -o VulkanTest.out main.cpp $(LDFLAGS)

.PHONY: test clean

test: VulkanTest
	./VulkanTest.out

clean:
	rm -f VulkanTest.out
