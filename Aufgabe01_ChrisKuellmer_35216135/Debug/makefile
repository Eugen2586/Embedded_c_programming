################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F4xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
Aufgabe01_ChrisKuellmer_35216135.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
Aufgabe01_ChrisKuellmer_35216135.list \

OBJCOPY_BIN += \
Aufgabe01_ChrisKuellmer_35216135.bin \


# All Target
all: Aufgabe01_ChrisKuellmer_35216135.elf secondary-outputs

# Tool invocations
Aufgabe01_ChrisKuellmer_35216135.elf: $(OBJS) $(USER_OBJS) C:\Users\Christian\Desktop\Projektarbeit_Embedded_C\Embedded_c_programming_blinken_mit_10_hz\Aufgabe01_ChrisKuellmer_35216135\STM32F446RETX_FLASH.ld
	arm-none-eabi-gcc -o "Aufgabe01_ChrisKuellmer_35216135.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m4 -T"C:\Users\Christian\Desktop\Projektarbeit_Embedded_C\Embedded_c_programming_blinken_mit_10_hz\Aufgabe01_ChrisKuellmer_35216135\STM32F446RETX_FLASH.ld" --specs=nosys.specs -Wl,-Map="Aufgabe01_ChrisKuellmer_35216135.map" -Wl,--gc-sections -static --specs=nano.specs -mfpu=fpv4-sp-d16 -mfloat-abi=hard -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

Aufgabe01_ChrisKuellmer_35216135.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "Aufgabe01_ChrisKuellmer_35216135.list"
	@echo 'Finished building: $@'
	@echo ' '

Aufgabe01_ChrisKuellmer_35216135.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "Aufgabe01_ChrisKuellmer_35216135.bin"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST) $(OBJCOPY_BIN)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
