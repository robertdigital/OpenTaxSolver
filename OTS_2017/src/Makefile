# SPDX-License-Identifier: GPL-2.0-or-later

CC = gcc
CFLAGS += -O -Wall
BUILD = ../bin

.PHONY: all
all: $(BUILD)/taxsolve_US_1040_2017 \
	$(BUILD)/taxsolve_US_1040_Sched_C_2017 \
	$(BUILD)/taxsolve_PA_40_2017 \
	$(BUILD)/taxsolve_NJ_1040_2017 \
	$(BUILD)/taxsolve_VA_760_2017 \
	$(BUILD)/taxsolve_NC_D400_2017 \
	$(BUILD)/taxsolve_OH_IT1040_2017 \
	$(BUILD)/taxsolve_NY_IT201_2017 \
	$(BUILD)/taxsolve_MA_1_2017 \
	$(BUILD)/taxsolve_CA_540_2017 \
	$(BUILD)/universal_pdf_file_modifier \
	$(BUILD)/convert_results2xfdf \
	../Run_taxsolve_GUI

$(BUILD)/taxsolve_US_1040_2017: taxsolve_US_1040_2017.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_US_1040_Sched_C_2017: taxsolve_US_1040_Sched_C_2017.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_CA_540_2017: taxsolve_CA_540_2017.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_NC_D400_2017: taxsolve_NC_D400_2017.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_PA_40_2017: taxsolve_PA_40_2017.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_NJ_1040_2017: taxsolve_NJ_1040_2017.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_OH_IT1040_2017: taxsolve_OH_IT1040_2017.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_VA_760_2017: taxsolve_VA_760_2017.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_NY_IT201_2017: taxsolve_NY_IT201_2017.c #taxsolve_routines.c
	@mkdir -p $(BUILD)
	$(CC) $(CFLAGS) -o $@ $^

$(BUILD)/taxsolve_MA_1_2017: taxsolve_MA_1_2017.c #taxsolve_routines.c
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
