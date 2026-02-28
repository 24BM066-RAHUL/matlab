1. Introduction

Biomedical signals such as ECG (Electrocardiogram), EEG (Electroencephalogram), and EMG (Electromyogram) contain sensitive patient health information. With the growth of telemedicine, IoT-based healthcare systems, and remote patient monitoring, these signals are frequently transmitted over wireless networks.

However, transmitting medical data over public or unsecured networks makes it vulnerable to:

Unauthorized access

Data tampering

Privacy violations

Cyber-attacks

Therefore, secure encryption techniques are required to protect biomedical signals during transmission.

This project presents a MATLAB-based simulation of encrypting and decrypting ECG signals using AES (Advanced Encryption Standard) to ensure secure transmission.

2. Objective

The main objective of this project is:

To implement encryption on real ECG signals.

To simulate secure transmission of biomedical data.

To decrypt the signal at the receiver side.

To analyze performance using security metrics such as MSE and PSNR.

3. Methodology

The simulation consists of the following stages:

Step 1: Data Acquisition

The PTB Diagnostic ECG dataset is loaded in MATLAB. The ECG signal is extracted from the dataset while removing the label column.

Step 2: Signal Preprocessing

The ECG signal is normalized between 0 and 1 and converted into an 8-bit integer format to make it suitable for encryption.

Step 3: AES Encryption

AES-128 symmetric key encryption is applied using a 16-byte secret key.
The encrypted output appears completely random, ensuring confidentiality.

Step 4: Secure Transmission Simulation

The encrypted signal is considered transmitted over a communication channel.

Step 5: Decryption

At the receiver side, the same AES key is used to decrypt the signal and recover the original ECG waveform.

Step 6: Performance Evaluation

To verify accuracy:

Mean Square Error (MSE) is calculated.

Peak Signal-to-Noise Ratio (PSNR) is computed.

A low MSE and high PSNR indicate successful recovery.

4. Tools and Technologies Used

MATLAB Software

PTB Diagnostic ECG Dataset

AES-128 Encryption Algorithm

Java Cryptography Library (Integrated with MATLAB)

5. Results

The encrypted ECG signal appears noise-like and unreadable.

The decrypted signal closely matches the original signal.

MSE value is approximately near zero.

PSNR value is high (indicating accurate reconstruction).

This confirms that the encryption and decryption process works effectively without signal distortion.

6. Applications

This system can be used in:

Telemedicine systems

Remote patient monitoring

Wearable health devices

IoT-based smart healthcare

Hospital data protection systems

7. Advantages

Ensures patient data confidentiality

Prevents unauthorized access

Maintains signal integrity

Easy implementation using MATLAB

8. Conclusion

The MATLAB simulation successfully demonstrates secure transmission of biomedical ECG signals using AES encryption. The encrypted signal protects sensitive medical information during transmission, and the decrypted signal accurately reconstructs the original waveform.

This approach can be extended to real-time healthcare systems for secure biomedical communication.
