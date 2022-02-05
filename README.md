# Java_GUI
In this repository I included basic logical programs written in java.


package login_system;

import java.awt.EventQueue;

import javax.swing.JFrame;
import java.awt.Color;
import java.awt.Font;
import java.awt.Window.Type;
import javax.swing.JLabel;
import javax.swing.JTextField;
import javax.swing.JButton;
import javax.swing.JSeparator;
import java.awt.event.ActionListener;
import java.awt.event.ActionEvent;
import java.awt.event.FocusAdapter;
import java.awt.event.FocusEvent;

public class square {

	private JFrame frmJyotisFirstLogin;
	private JTextField txtEnterTheNumber;
	private JTextField txtResult;
	private JTextField textField;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					square window = new square();
					window.frmJyotisFirstLogin.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the application.
	 */
	public square() {
		initialize();
	}

	/**
	 * Initialize the contents of the frame.
	 */
	private void initialize() {
		frmJyotisFirstLogin = new JFrame();
		frmJyotisFirstLogin.setBackground(new Color(0, 0, 0));
		frmJyotisFirstLogin.setType(Type.POPUP);
		frmJyotisFirstLogin.setTitle("jyoti's first login pop up box");
		frmJyotisFirstLogin.getContentPane().setFont(new Font("Tahoma", Font.BOLD, 14));
		frmJyotisFirstLogin.getContentPane().setForeground(new Color(255, 69, 0));
		frmJyotisFirstLogin.getContentPane().setBackground(new Color(46, 139, 87));
		frmJyotisFirstLogin.setBounds(100, 100, 508, 528);
		frmJyotisFirstLogin.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		frmJyotisFirstLogin.getContentPane().setLayout(null);
		
		JLabel lblNewLabel = new JLabel("FINDING SQUARE");
		lblNewLabel.setBackground(Color.DARK_GRAY);
		lblNewLabel.setFont(new Font("Tw Cen MT", Font.BOLD, 30));
		lblNewLabel.setForeground(Color.YELLOW);
		lblNewLabel.setBounds(22, 25, 406, 49);
		frmJyotisFirstLogin.getContentPane().add(lblNewLabel);
		
		JLabel lblNewLabel_1 = new JLabel("NUMBER  :  ");
		lblNewLabel_1.setForeground(Color.YELLOW);
		lblNewLabel_1.setFont(new Font("Trebuchet MS", Font.BOLD, 20));
		lblNewLabel_1.setBounds(22, 125, 127, 38);
		frmJyotisFirstLogin.getContentPane().add(lblNewLabel_1);
		
		txtEnterTheNumber = new JTextField();
		txtEnterTheNumber.setForeground(Color.GRAY);
		txtEnterTheNumber.setText("ENTER THE NUMBER ");
		txtEnterTheNumber.setFont(new Font("Tempus Sans ITC", Font.ITALIC, 18));
		txtEnterTheNumber.setBounds(172, 134, 196, 23);
		frmJyotisFirstLogin.getContentPane().add(txtEnterTheNumber);
		txtEnterTheNumber.setColumns(10);
		
		txtResult = new JTextField();
		txtResult.setForeground(Color.GRAY);
		txtResult.setText("ENTER THE POWER");
		txtResult.setFont(new Font("Tempus Sans ITC", Font.ITALIC, 18));
		txtResult.setColumns(10);
		txtResult.setBounds(172, 207, 196, 23);
		frmJyotisFirstLogin.getContentPane().add(txtResult);
		
		JLabel lblNewLabel_1_1 = new JLabel("POWER");
		lblNewLabel_1_1.setForeground(Color.YELLOW);
		lblNewLabel_1_1.setFont(new Font("Trebuchet MS", Font.BOLD, 20));
		lblNewLabel_1_1.setBounds(22, 198, 127, 38);
		frmJyotisFirstLogin.getContentPane().add(lblNewLabel_1_1);
		
		JButton btnNewButton = new JButton("SHOW");
		btnNewButton.setForeground(Color.BLUE);
		btnNewButton.setBackground(Color.LIGHT_GRAY);
		btnNewButton.setFont(new Font("Tw Cen MT", Font.ITALIC, 15));
		btnNewButton.setBounds(217, 366, 89, 23);
		frmJyotisFirstLogin.getContentPane().add(btnNewButton);
		
		JButton btnExit = new JButton("EXIT");
		btnExit.addFocusListener(new FocusAdapter() {
			@Override
			public void focusGained(FocusEvent e) {
			}
		});
		btnExit.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent arg0) {
				System.exit(0);
			}
		});
		btnExit.setForeground(Color.RED);
		btnExit.setFont(new Font("Tw Cen MT", Font.ITALIC, 15));
		btnExit.setBackground(new Color(192, 192, 192));
		btnExit.setBounds(217, 408, 89, 23);
		frmJyotisFirstLogin.getContentPane().add(btnExit);
		
		JSeparator separator = new JSeparator();
		separator.setForeground(Color.DARK_GRAY);
		separator.setBounds(22, 87, 445, 2);
		frmJyotisFirstLogin.getContentPane().add(separator);
		
		JSeparator separator_1 = new JSeparator();
		separator_1.setForeground(Color.DARK_GRAY);
		separator_1.setBounds(22, 339, 445, 2);
		frmJyotisFirstLogin.getContentPane().add(separator_1);
		
		JLabel lblNewLabel_1_1_1 = new JLabel("RESULT  :");
		lblNewLabel_1_1_1.setForeground(Color.YELLOW);
		lblNewLabel_1_1_1.setFont(new Font("Trebuchet MS", Font.BOLD, 20));
		lblNewLabel_1_1_1.setBounds(22, 273, 127, 38);
		frmJyotisFirstLogin.getContentPane().add(lblNewLabel_1_1_1);
		
		textField = new JTextField();
		textField.setForeground(Color.GRAY);
		textField.setText("RESULT");
		textField.setFont(new Font("Tempus Sans ITC", Font.ITALIC, 18));
		textField.setColumns(10);
		textField.setBounds(172, 282, 196, 23);
		frmJyotisFirstLogin.getContentPane().add(textField);
	}
}
