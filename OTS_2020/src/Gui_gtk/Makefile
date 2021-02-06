# SPDX-License-Identifier: GPL-2.0-or-later

CC = gcc
BUILD ?= ../../bin
CFLAGS += -O -Wall
GTK2_FLAGS = -Wno-deprecated-declarations `pkg-config --cflags gtk+-2.0`
GTK2_LIBS = `pkg-config --libs gtk+-2.0`

.PHONY: all
all:  $(BUILD)/ots_gui2

$(BUILD)/ots_gui2: ots_gui2.c #gtk_utils.c gtk_file_browser.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) $(GTK2_FLAGS) -o $@ $^ $(GTK2_LIBS)

.PHONY: clean
clean:
	$(RM) $(BUILD)/ots_gui2
