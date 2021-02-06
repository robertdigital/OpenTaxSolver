# SPDX-License-Identifier: GPL-2.0-or-later

CC = gcc
CFLAGS += -O -Wall
BUILD = ../bin

.PHONY: all
all: $(BUILD)/taxsolve_US_1040_2018 \
	$(BUILD)/taxsolve_US_1040_Sched_C_2018 \
	$(BUILD)/taxsolve_PA_40_2018 \
	$(BUILD)/taxsolve_NJ_1040_2018 \
	$(BUILD)/taxsolve_VA_760_2018 \
	$(BUILD)/taxsolve_NC_D400_2018 \
	$(BUILD)/taxsolve_OH_IT1040_2018 \
	$(BUILD)/taxsolve_NY_IT201_2018 \
	$(BUILD)/taxsolve_MA_1_2018 \
	$(BUILD)/taxsolve_CA_540_2018 \
	$(BUILD)/universal_pdf_file_modifier \
	$(BUILD)/convert_results2xfdf \
	../Run_taxsolve_GUI

$(BUILD)/taxsolve_US_1040_2018: taxsolve_US_1040_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_US_1040_Sched_C_2018: taxsolve_US_1040_Sched_C_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_CA_540_2018: taxsolve_CA_540_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_NC_D400_2018: taxsolve_NC_D400_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_PA_40_2018: taxsolve_PA_40_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_NJ_1040_2018: taxsolve_NJ_1040_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_OH_IT1040_2018: taxsolve_OH_IT1040_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_VA_760_2018: taxsolve_VA_760_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_NY_IT201_2018: taxsolve_NY_IT201_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_MA_1_2018: taxsolve_MA_1_2018.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/universal_pdf_file_modifier: universal_pdf_file_modifier.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/convert_results2xfdf: convert_results2xfdf.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

../Run_taxsolve_GUI: Run_taxsolve_GUI.c
	$(CC) $(CFLAGS) -o $@ $^

.PHONY: clean
clean:
	$(RM) -rv $(BUILD) ../Run_taxsolve_GUI
